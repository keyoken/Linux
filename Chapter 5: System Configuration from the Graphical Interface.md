# Chapter 5: System Configuration from the Graphical Interface


#### Learning Objectives

By the end of this chapter, you should be able to:

* Apply system, display, and date and time settings using the System Settings panel.
* Track the network settings and manage connections using Network Manager in Linux.
* Install and update software in Linux from a graphical interface.

### System Settings

The System Settings panel allows you to control most of the basic configuration options and desktop settings, such as specifying the screen resolution, managing network connections, or changing the date and time of the system.

For the GNOME Desktop Manager, one clicks on the upper right-hand corner and then selects the tools image (screwdriver crossed with a wrench or a gear). Depending on your distribution, you may find other ways to get into the settings configuration as well.


###Date and Time Settings

By default, Linux always uses Coordinated Universal Time (UTC) for its own internal timekeeping. Displayed or stored time values rely on the system time zone setting to get the proper time. UTC is similar to, but more accurate than, Greenwich Mean Time (GMT).

If you click on the time displayed on the top panel, you can adjust the format with which the date and time is shown; on some distributions, you can also alter the values.

The more detailed date and time settings can from the System  ***Settings->Details->Date & Time window.***

### Network Time Protocol
The Network Time Protocol (NTP) is the most popular and reliable protocol for setting the local time by consulting established Internet servers. Linux distributions always come with a working NTP setup, which refers to specific time servers run or relied on by the distribution. This means that no setup, beyond "on" or "off", is required for network time synchronization. If desired, more detailed configuration is possible by editing the standard NTP configuration file (/etc/ntp.conf) for Linux NTP utilities.



### Lab 5.1: Getting and Setting Screen Resolution
Note: You can also ascertain your current resolution by typing at the command line:

``` student:/tmp> $ xdpyinfo | grep dim
    dimensions: 3200x1080 pixels (847x286 millimeters)
```


### Network Configuration

All Linux distributions have network configuration files, but file formats and locations can differ from one distribution to another. Hand editing of these files can handle quite complicated setups, but is not very dynamic or easy to learn and use. Network Manager was developed to make things easier and more uniform across distributions. It can list all available networks (both wired and wireless), allow the choice of a wired, wireless, or mobile broadband network, handle passwords, and set up Virtual Private Networks (VPNs). Except for unusual situations, it is generally best to let Network Manager establish your connections and keep track of your settings.



###Mobile Broadband and VPN Connections
You can set up a mobile broadband connection with Network Manager, which will launch a wizard to set up the connection details for each connection.
Once the configuration is done, the network is configured automatically each time the broadband network is attached.
Network Manager can also manage your VPN connections.
It supports many VPN technologies, such as native IPSec, Cisco OpenConnect (via either the Cisco client or a native open source client), Microsoft PPTP, and OpenVPN.
You might get support for VPN as a separate package from your distributor. You need to install this package if your preferred VPN is not supported.


### Installing and Updating Software

Each package in a Linux distribution provides one piece of the system, such as the Linux kernel, the C compiler, the shared software code for interacting with USB devices, or the Firefox web browser.
Packages often depend on each other. For example, because Firefox can communicate using SSL/TLS, it will depend on a package which provides the ability to encrypt and decrypt SSL and TLS communication, and will not install unless that package is also installed at the same time.

All systems have a lower-level utility which handles the details of unpacking a package and putting the pieces in the right places. Most of the time, you will be working with a higher-level utility which knows how to download packages from the Internet and can manage dependencies and groups for you.


### Debian Packaging
Let’s look at the Package Management for the Debian family system.

dpkg is the underlying package manager for these systems. It can install, remove, and build packages. Unlike higher-level package management systems, it does not automatically download and install packages and satisfy their dependencies.

For Debian-based systems, the higher-level package management system is the Advanced Package Tool (APT) system of utilities. Generally, while each distribution within the Debian family uses APT, it creates its own user interface on top of it (for example, apt, apt-get, aptitude, synaptic, Ubuntu Software Center, Update Manager, etc). Although apt repositories are generally compatible with each other, the software they contain generally is not. Therefore, most repositories target a particular distribution (like Ubuntu), and often software distributors ship with multiple repositories to support multiple distributions. 


### Red Hat Package Manager (RPM)
Red Hat Package Manager (RPM) is the other package management system popular on Linux distributions. It was developed by Red Hat, and adopted by a number of other distributions, including SUSE/penSUSE, Mageia, CentOS, Oracle Linux, and others.

The higher-level package manager differs between distributions: Red Hat family distributions historically used the repository ***format used by yum*** , however, RHEL/CentOS 8 and Fedora have moved over to using dnf, which is mostly backwards compatible with yum. SUSE family distributions also use RPM, but use the zypper interface. The GNOME project also uses PackageKit as a unified interface.


### Summary
You have completed Chapter 5. Let's summarize the key concepts covered:

* You can control basic configuration options and desktop settings through the System Settings panel.
* Linux always uses Coordinated Universal Time (UTC) for its own internal time-keeping. You can set the date and time settings from the System Settings window.
* The Network Time Protocol is the most popular and reliable protocol for setting the local time via Internet servers.
* The Displays panel allows you to change the resolution of your display and configure multiple screens.
* Network Manager can present available wireless networks, allow the choice of a wireless or mobile broadband network, handle passwords, and set up VPNs.
* ***dpkg and RPM*** are the most popular package management systems used on Linux distributions.
* Debian distributions use dpkg and apt-based utilities for package management.
* RPM was developed by Red Hat, and adopted by a number of other distributions, including the openSUSE, Mandriva, CentOS, Oracle Linux, and others.
