The Linux file tree
======================

### 1. **Filesystem hierarchy standard**

Many Linux distributions partially follow the Filesystem Hierarchy Standard (FHS). The FHS may help make more Unix/Linux file system trees conform better in the future.     
It is possible to define two independent distinctions among files: shareable vs. unshareable and variable vs. static. In general, files that differ in either of these respects should be located in different directories. This makes it easy to store files with different usage characteristics on different filesystems.  
"Shareable" files are those that can be stored on one host and used on others. "Unshareable" files are those thatare not shareable. For example, the files in user home directories are shareable whereas device lock files are not.  
"Static" files include binaries, libraries, documentation files and other files that do not change without system administrator intervention. "Variable" files are files that are not static.  
Shareable files can be stored on one host and used on several others. Typically, however, not all files in the filesystem hierarchy are shareable and so each system has local storage containing at least its unshareable files. It is convenient if all the files a system requires that are stored on a foreign host can be made available by mounting one or a few directories from the foreign host.
