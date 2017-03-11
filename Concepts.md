## Device file
In UNIX-like operating systems, a device file or special file is an interface for a device driver that appear in a file system as if it were an ordinary file. They allows software to interact with a device driver using standard input/output system calls, which simplifies many tasks and unifies user-space I/O mechanism.  
There are two general kinds of devices files in Unix-like operating system, known as character special files and block special files. The difference between them lies in how data written to them and read from them is processed by the operating system and hardware. These together can be called device special files in contrast to named pipes, which are not connected to a device but are not ordinary files either.  
Device nodes correspond to resources that an operating system's kernel has already allocated. Unix identifies those resources by a major number and a minor number, both stored as part of the structure of node. The assignment of these numbers occurs uniquely in different operating systems and on different computer platforms. Gennerally, the major number identifies the device driver and the minor number identifies a particular device (possibly out of many) that the dirver controls: in this case, the system may pass the minor number to a driver.  
As with other special file types, the computer system accesses device nodes using standard system calls and treats them like regular computer files. Two standard types of device files exist; unfortunately their names are, for historical reasons, rather counter-intuitive, and explanations of the difference between the two are often incorrect as a result.  
### Character devices  
Character special files or character devices provide unbuffered, direct access to hardware device. They do not necessarily allow programs to read or write single characters at a time; that is up to the divice in question. The character divice for a hard disk, for example, will normally require that all reads and writes are aligned to block boundaries and most certainly will not allow reading a single byte.  
Character devices are sometimes known as raw diveces to avoid the confusion surrounding the fact that a character device for a piece of block-based hardware will typically require programs to read and write aligned blocks.  
### Block devices  
Block special files or block devices provide buffered accesses to hardware devices, and provide some abstraction from their specifics. Unlike character devices, block devices will always allow the programmer to read or write a block of any size (including single characters/bytes) and any alignment. The downside is that because block devices are buffered, the programer does not know  how long it will take before written date is passed from the kernel's buffers to the actual device, or indeed in what order two separate writes will arrive at the physical device; additionally, if the same hardware exposes both character and block devices, ther is a risk of data corruption due to client using the character device being unaware of changes made in the buffers of the block device.  
Most systems create both block and charater devices to represent hardware like hardisks. FreeBSD and Linux notably do not; the former has removed support for block devices, while the latter creates only block devices. In Linux, to get character device for a disk one must use the "raw" driver, though one can get the same effect as opening a character device by opening the block device with the Linux-specific 0_DIRECT flag.  
### Pseudo-devices  
Device nodes on Unix-like systems do not necessarily have to correspond to physical devices. Nodes that lack this correspondence form the group of pseudo-devices. They provide various function handled by the operating system. Some of the most commonly used (character-based) pseudo-devices include:  
* /dev/null
* /dev/zero
* /dev/full
* /dev/random
* /dev/urandom



