Introduction to Linux
======================

#### 1. **Linux history**

All modern operating systems have their roots in 1969 when Dennis Ritchie and Ken Thompson developed the C language and the Unix OS at AT&T lab. They shared their source code with the rest of the world. By 1975, when AT&T started selling Unix commercially, about half of the source code was written by the others. Many people who had contributed to Unix were not happy that the commercial company sold the software that had been written by them. The battle between AT&T and these people ended with two version of Unix: the official AT&T Unix and the free **BSD** Unix  
Development of BSD descendants like FreeBSD, OpenBSD, NetBSD, DragonFly BSD and PC-BSD is still active today.  

In the 1980s, many company created their own Unix, IBM created AIX, Sun: SunOS (later: Solaris), HP: HP-UX and about dozen other companies did the same. The result is a mess of Unix dialects and a dozen of different ways to do the same thing. And here is the first real root of Linux, when Richart Stallman aimed to end this era of Unix separation and everybody re-inventing the wheel by   
starting the **GNU** project. His aim was to make an operating system that freely available to everyone and where everyone could work together. Many of the commandline tools that you use on Linux today is GNU tools.  

The Nineties started with Linus Torvalds, a Swedish speaking Finnish student, buying a 386  computer  and  writing  a  brand  new  POSIX compliant kernel. He put the source code online, thinking it would never support anything but 386 hardware. Many people embraced the combination of this kernel with the GNU tools, and the rest, as they say, is history.  

Today more than 97 percent of the world's supercomputers (including the complete top 10), more than 80 percent of all smartphones, many millions of desktop computers, around 70 percent of all web servers, a large chunk of tablet computers, and several appliances (dvd-players, washing machines, dsl modems, routers, self-driving cars, space station laptops...) run Linux. Linux is by far the most commonly used operating system in the world. Linux kernel version 4.0 was released in April 2015. Its source code grew by several hundred thousand lines (compared to version 3.19 from February 2015) thanks to contributions of thousands of developers  paid  by  hundreds  of  commercial  companies  including  Red  Hat, Intel,  Samsung,  Broadcom,  Texas  Instruments,  IBM,  Novell,  Qualcomm,  Nokia,  Oracle, Google, AMD and even Microsoft (and many more).

#### 2. **Distributions**

A Linux distribution is a collection of (usually open source) software on top of a Linuxkernel. A distribution (or short, distro) can bundle server software, system  management tools,  documentation and many desktop  applications in a central secure software
repository. A distro aims to  provide a common look and feel, secure and easy software management and often a specific operational purpose.  
Let's take a look at some popular distributions.

* Read Hat: Red Hat is a billion dollar commercial Linux company that puts a lot of effort in developing Linux. They have hundreds of Linux specialists and are known for their excellent support. They give their products (Red Hat Enterprise Linux and Fedora) away for free. While Red Hat Enterprise Linux (RHEL) is well tested before release and supported for up to sevenyears after release, Fedora is a distro with faster updates but without support.
* Ubuntu: Canonical started sending out free compact discs with Ubuntu Linux in 2004 and quickly became  popular  for  home  users  (many  switching  from  Microsoft  Windows).  Canonical wants  Ubuntu  to  be  an  easy  to  use  graphical  Linux  desktop without need to ever see a command line. Of course they also want to make a profit by selling support for Ubuntu.
* Debian: There is no company behind Debian. Instead there are thousands of well organised developers that elect a Debian Project Leader every two years. Debian is seen as one of the most stable Linux distributions. It is also the basis of every release of Ubuntu. Debian comes in three versions: stable, testing and unstable. Every Debian release is named after a character in the movie Toy Story.
* Other: Distributions like CentOS, Oracle Enterprise Linux and Scientific Linux are  based  on Red  Hat  Enterprise  Linux  and  share  many  of  the  same  principles,  directories  and system  administration  techniques. Linux  Mint, Edubuntu and  many  other  \*buntu  named distributions are based on Ubuntu and thus share a lot with Debian. There are hundreds of other Linux distributions.  

#### 3. **Licensing**

##### 3.1 **About software licenses**

There are two predominant software paradigms: Free and Open Source Software (FOSS) and proprietary software. The criteria for differentiation between these two approaches is based on control over the software. With proprietary software, control tends to lie more with the vendor, while with Free and Open Source Software it tends to be more weighted towards the end user. But even though the paradigms differ, they use the same copyright laws to reach and enforce their goals. From a legal perspective, Free  and  Open  Source Software can be considered as software to which users generally receive more rights via their license agreement than they would have with a proprietary software license, yet the underlying license mechanisms are the same.  
Legal theory states that the author of FOSS, contrary to the author of public domain software, has in no way whatsoever given up his rights on his work. FOSS supports on the rights of the author (the copyright) to impose FOSS license conditions. The FOSS license conditions need to be respected by the user in the same way as proprietary license conditions. Always check your license carefully before you use third party software.  
Examples of proprietary software are AIX from IBM, HP-UX from HP and Oracle Database 11g. You are not authorised to install  or  use this software without paying a licensing fee. You are not authorised to distribute copies and you are not authorised to modify the closed source code.

##### 3.2 **Public domain software and freeware**

Software that is original in the sense that it is an intellectual creation of the author benefits copyright protection.Non-original software does not come into consideration for copyright protection and can, in principle, be used freely.  
Public domain software is considered as software to which the author has given up all rights and on which nobody is able to enforce any rights. This software can be used, reproduced or executed freely, without permission or the payment of a fee. Public domain software can in certain cases even be presented by third parties as own work, and by modifying the original work, third parties can take certain versions of the public domain software out of the public domain again.  
Freeware is not public domain software or FOSS. It is proprietary software that you can use without paying a license cost. However, the often strict license terms need to be respected.  
Examples of freeware are Adobe Reader, Skype and Command and Conquer: Tiberian Sun (this game was sold as proprietary in 1999 and is since 2011 available as freeware).  

##### 3.3 **Free Software or Open Source Software**

Both the Free Software and the Open Source Software movement largely pursue similar goals and endorse similar software licenses. But historically, there has been some perception of differentiation due to different emphases. Where the Free Software movement focuses on the rights (the four freedoms) which Free Software provides to its users, the Open Source Software movement points to its Open Source Definition and the advantages of peer-to-peer software development.  
Recently, the term free and open source software or FOSS has arisen as a neutral alternative. A lesser-used variant is free/libre/open source software (FLOSS), which uses libre to clarify the meaning of free as in freedom rather than as in at no charge.  
Examples of free software are gcc, MySQL and gimp.  

##### 3.3 **Using GPLv3 software**

You can use GPLv3 software almost without any conditions. If you solely run the software you even don’t have to accept the terms of the GPLv3. However, any other use - such as modifying or distributing the software - implies acceptance.  
In case you use the software internally (including over a network), you may modify the software without being obliged to distribute your modification. You may hire third parties to work on the software exclusively for you and under your direction and control. But if you modify the software and use it otherwise than merely internally, this will be considered as distribution. You must distribute your modifications under GPLv3 (the copyleft principle). Several more obligations apply if you distribute GPLv3 software. Check the GPLv3 license carefully.  
You create output with GPLv3 software: The GPLv3 does not automatically apply to the output.  

##### 3.3 **BSD license**

There are several versions of the original Berkeley Distribution License. The most common one is the 3-clause license ("New BSD License" or "Modified BSD License").  
This is a permissive free software license. The license places minimal restrictions on how the software can be redistributed. This is in contrast to copyleft licenses such as the GPLv. 3 discussed above, which have a copyleft mechanism.  
This difference is of less importance when you merely use the software, but kicks in when you start redistributing verbatim copies of the software or your own modified versions.
