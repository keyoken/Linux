# Chapter 2: Linux Philosophy and Concepts

Three Important Pieces of Context

Please keep in mind the following:

1. Things change in Linux
No matter how hard we have worked to stay current, Linux is constantly evolving, both at the technical level (including kernel features) and at the distribution and interface level. So, please keep in mind we have tried to be as up-to-date as possible at the time this course was released, but there may be changes and new features we have not discussed. This is unavoidable.


2. We have repeated some things in the class material
It is just about impossible in a course this comprehensive to never revisit topics that have previously been covered, and short reviews are helpful so you do not have to go scouring through earlier sections to jog your memory. This is particularly true with system configuration items, like how to use sudo to gain temporary root privileges in as safe a manner as possible. We know we have done this and, at least in most cases, it is by design, not by accident.

3. We have tried to avoid holy wars
There are many areas where there are strong preference disagreements in the Linux (and wider open source) community. Examples include the best editor: emacs vs. vi; the best graphical desktop: GNOME vs. KDE, etc. Usually, we have chosen (when necessary) a particular alternative to emphasize just to keep things clean. For example, we talk much more about GNOME than KDE simply because it has a bigger user base, not because we are taking a position as to which is superior.


### Learning Objectives

By the end of this chapter, you should be able to:

* Discuss the history and philosophy of Linux.
* Describe the Linux community.
* Define the common terms associated with Linux.
* Discuss the components of a Linux distribution.

### History

Linux is an open source computer operating system, initially developed on and for Intel x86-based personal computers. It has been subsequently ported to an astoundingly long list of other hardware platforms, from tiny embedded appliances to the world's largest supercomputers.
In this section, we follow the surprising history of how Linux evolved from a project of one Finnish college student, into a massive effort with an enormous impact on today's world.

Linus Torvalds was a student in Helsinki, Finland, in 1991, when he started a project: writing his own operating system kernel. He also collected together and/or developed the other essential ingredients required to construct an entire operating system with his kernel at the center. It wasn't long before this became known as the Linux kernel. 
In 1992, Linux was re-licensed using the General Public License (GPL) by GNU (a project of the Free Software Foundation or FSF, which promotes freely available software), which made it possible to build a worldwide community of developers. By combining the kernel with other system components from the GNU project, numerous other developers created complete systems called Linux distributions in the mid-90’s.



### Linux Philosophy

Linux borrows heavily from the well-established UNIX operating system. 
It was written to be a free and open source system to be used in place of UNIX, which at the time was designed for computers much more powerful than PCs and was quite expensive. 
Files are stored in a hierarchical filesystem, with the top node of the system being the root or simply "/". 
Whenever possible, Linux makes its components available via files or objects that look like files. Processes, devices, and network sockets are all represented by file-like objects, and can often be worked with using the same utilities used for regular files.
Linux is a fully multitasking (i.e. multiple threads of execution are performed simultaneously), multiuser operating system, with built-in networking and service processes known as daemons in the UNIX world.

 **Note: Linux was inspired by UNIX, but it is not UNIX.**


The Linux community is a far-reaching ecosystem consisting of developers, system administrators, users and vendors who use many different forums to connect with one another. Among the most popular are:

Internet Relay Chat (IRC) software (such as WeeChat, HexChat, Pidgin and XChat)
Online communities and discussion boards including Linux User Groups (both local and online)
Many collaborative projects hosted on services such as GitHub
Newsgroups and mailing lists, including the Linux Kernel Mailing List
Community events, e.g. Hackathons, Install Fests, Open Source Summits and Embedded Linux Conferences.
A portal to one of the most powerful online user communities can be found at linux.com. This site is hosted by The Linux Foundation and serves over one million unique visitors every month. It has active sections on:

 
 
 
 ### Linux Terminology
Basic Terms such as kernel, distribution, boot loader, service, filesystem, X Window system, desktop environment, and command line.
 
The kernel is considered the brain of the Linux operating system. 
A distribution also known as Distros is a collection of programs combined with the Linux kernel to make up a Linux-based operating system.
The boot loader, as the name implies, is a program that boots the operating system. Two examples of a boot loader are GRUB and ISOLINUX.
A service is a program that runs as a background process. Some examples of the service are httpd, nfsd, ntpd, ftpd and named.
A filesystem is a method for storing and organizing files in Linux. Some examples of filesystems are ext3, ext4, FAT, XFS and Btrfs.
The X Window System provides the standard toolkit and protocol to build graphical user interfaces on nearly all Linux systems.
The desktop environment is a graphical user interface on top of the operating system. GNOME, KDE, Xfce and Fluxbox are some examples of the desktop environment.
The command line is an interface for typing commands on top of the operating system.
The Shell is the command line interpreter that interprets the command line input and instructs the operating system to perform any necessary tasks and commands. 
For example, bash, tcsh and zsh.


### Linux Distributions

 A full Linux distribution consists of the kernel plus a number of other software tools for file-related operations, user management, and software package management. Each of these tools provides a part of the complete system. Each tool is often its own separate project, with its own developers working to perfect that piece of the system.
 
 
 
 ### Summary
 
 **You have completed Chapter 2.***
 
 Let’s summarize the key concepts covered:

* Linux borrows heavily from the UNIX operating system, with which its creators were well-versed.
* Linux accesses many features and services through files and file-like objects.
* Linux is a fully multi-tasking, multi-user operating system, with built-in networking and service processes known as daemons.
* Linux is developed by a loose confederation of developers from all over the world, collaborating over the Internet, with Linus Torvalds at the head. 
* Technical skill and a desire to contribute are the only qualifications for participating.
* The Linux community is a far reaching ecosystem of developers, vendors, and users that supports and advances the Linux operating system.
* Some of the common terms used in Linux are: kernel, distribution, boot loader, service, filesystem, X Window system, desktop  environment, and command line.
* A full Linux distribution consists of the kernel plus a number of other software tools for file-related operations, user management, and software package management.
