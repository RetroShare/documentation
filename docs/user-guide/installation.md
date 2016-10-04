#RetroShare is available for various Operating Systems. 

##Windows
![windows logo](../img/install/windows_logo.png "Windows Install")  

The installers for Windows contains the portable and normal install, and plugins.  
Links:   

 - [Retroshare-0.6.1-Qt4](https://github.com/RetroShare/RetroShare/releases/download/0.6.1/RetroShare-0.6.1-20160903-53e26983-Qt4-setup.exe) Installer  
 - [Retroshare-0.6.1-Qt5](https://github.com/RetroShare/RetroShare/releases/download/0.6.1/RetroShare-0.6.1-20160903-53e26983-Qt5-setup.exe) Installer  

The installers for Windows contains the portable and normal install, and plugins.  
Checksums: [checksum.txt](https://github.com/RetroShare/RetroShare/releases/download/0.6.1/chksums.txt.asc)


##Apple
![apple logo](../img/install/apple_logo.png "Apple Install")  

RetroShare is currently available for MacOS (v0.6.0 only, on Sept 3, 2016. 0.6.1 coming soon!)

Link: [RetroShare_v0.6.0.dmg](https://github.com/RetroShare/RetroShare/releases/download/v0.6.0/Retroshare-0.6.0-OSX-20160209-4033f35f.dmg)  
Checksums: [checksum.txt](https://github.com/RetroShare/RetroShare/releases/download/v0.6.0/checksums.txt.asc)  


##Ubuntu
![ubuntu logo](../img/install/ubuntu_logo.png "Ubuntu Install")  

Retroshare is currently available on all Ubuntu distributions up to Xenial (16.04).

To install Retroshare on ubuntu, please use one of the following two PPA repositories

 - Stable: [retroshare stable](https://launchpad.net/~retroshare/+archive/ubuntu/stable)
 - Regular development releases: [retroshare unstable](https://launchpad.net/~retroshare/+archive/ubuntu/unstable)

Development releases are always tested and therefore reasonnably safe to use. They happen irregularly, with an average of 2 weeks between updates.

    # for Retroshare releases only
       sudo add-apt-repository ppa:retroshare/stable
    # for Retroshare development snapshots
       sudo add-apt-repository ppa:retroshare/unstable
    # then
       sudo apt-get update
       sudo apt-get install retroshare06

Since v0.6 and v0.5 networks are incompatible, we made sure that both versions can run simultaneously (hence the different package name for v0.6).

Packages for Ubuntu compatible for the Raspberry Pi are also available on GitHub


##Debian
![debian logo](../img/install/debian_logo.png "Debian Install")  

Retroshare is currently available on Debian Stretch for i386 and amd64 architectures.  
You can download packages from GitHub released by the Development Team: [Debian packages](https://github.com/RetroShare/RetroShare/releases/)  

Stable and Nightly Builds are also available here for Debian 7 Wheezy and Debian 8 Jessie:  
Stable: [retroshare](https://software.opensuse.org/download.html?project=home%3AAsamK%3ARetroShare&package=retroshare06)  
Nightly Builds: [retroshare-unstable](https://software.opensuse.org/download.html?project=home%3AAsamK%3ARetroShare&package=retroshare06-git)  

To receive RetroShare via your package manager, you can add the repository to your sources.

    # for Retroshare releases only
       sudo sh -c "echo 'deb http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/Debian_8.0/ /' >> /etc/apt/sources.list.d/retroshare06.list"
    # for Retroshare nightly builds
       sudo sh -c "echo 'deb http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/Debian_8.0/ /' >> /etc/apt/sources.list.d/retroshare06-git.list"
    # then
       sudo apt-get update
       sudo apt-get install retroshare06


##openSUSE
![opensuse logo](../img/install/opensuse_logo.png "openSUSE Install")  

Retroshare is currently available on openSUSE. 

Install stable release via: ![oneclick](../img/install/oneclick.png "yast oneclick Install")  

Download binary or add Repository manually:  

 - [Stable release](https://software.opensuse.org/download.html?project=home%3AAsamK%3ARetroShare&package=retroshare06) 
 - [Nightly snapshot](https://software.opensuse.org/download.html?project=home%3AAsamK%3ARetroShare&package=retroshare06-git)


###Stable openSUSE

**openSUSE Tumbleweed**  packages 

 - [retroshare06-0.6.1-3.7.i586.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/openSUSE_Tumbleweed/i586/retroshare06-0.6.1-3.7.i586.rpm)
 - [retroshare06-0.6.1-3.7.x86_64.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/openSUSE_Tumbleweed/x86_64/retroshare06-0.6.1-3.7.x86_64.rpm)  

**openSUSE Tumbleweed** repository  

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_Tumbleweed/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06

**openSUSE Leap 42.2**  packages

 - [retroshare06-0.6.1-3.1.x86_64.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/openSUSE_Leap_42.2/x86_64/retroshare06-0.6.1-3.1.x86_64.rpm)

**openSUSE Leap 42.2** repository  

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_Leap_42.2/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06

**openSUSE Leap 42.1** packages

 - [retroshare06-0.6.1-3.1.x86_64.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/openSUSE_Leap_42.1/x86_64/retroshare06-0.6.1-3.1.x86_64.rpm)

**openSUSE Leap 42.1** repository  

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_Leap_42.1/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06
       
**openSUSE Factory ARM** packages

 - [retroshare06-0.6.1-3.6.armv7hl.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/openSUSE_Factory_ARM/armv7hl/retroshare06-0.6.1-3.6.armv7hl.rpm)

**openSUSE Factory ARM** repository  

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_Factory_ARM/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06

**openSUSE 13.2** packages

 - [retroshare06-0.6.0-1.4.i586.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/openSUSE_13.2/i586/retroshare06-0.6.0-1.4.i586.rpm)
 - [retroshare06-0.6.0-1.4.x86_64.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/openSUSE_13.2/x86_64/retroshare06-0.6.0-1.4.x86_64.rpm)

**openSUSE 13.2** repository

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_13.2/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06

###Nightly Builds openSUSE

**openSUSE Tumbleweed**

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_Tumbleweed/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06-git

**openSUSE Leap 42.2**

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_Leap_42.2/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06-git

**openSUSE Leap 42.1**

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_Leap_42.1/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06-git

**openSUSE Factory ARM**

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_Factory_ARM/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06-git

**openSUSE 13.2**

       zypper addrepo http://download.opensuse.org/repositories/home:AsamK:RetroShare/openSUSE_13.2/home:AsamK:RetroShare.repo
       zypper refresh
       zypper install retroshare06-git

##Arch Linux
![archlinux logo](../img/install/arch_logo.png "Arch Install")  

RetroShare is currently available in Arch User Repository.  

 - Stable: [Arch User Repository](https://aur.archlinux.org/packages/retroshare/)  
 - Nightly Builds: [Arch User Repository](https://aur.archlinux.org/packages/retroshare-git/)

RetroShare Packages for Arch are also available on openSUSE Build Service

 - Stable: [OBS Stable](https://software.opensuse.org/download.html?project=home%3AAsamK%3ARetroShare&package=retroshare06)
 - Nighlty Builds: [OBS Nightly](https://software.opensuse.org/download.html?project=home%3AAsamK%3ARetroShare&package=retroshare06-git)

##Fedora
![fedora logo](../img/install/fedora_logo.png "Fedora Install")  

Retroshare is currently available on Fedora 23 and 24.

###Stable Fedora

 - Fedora 24 32bit [v0.6.1-3.1.i686.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/Fedora_24/i686/retroshare06-0.6.1-3.1.i686.rpm)   
 - Fedora 24 64bit [v0.6.1-3.1.x86_64.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/Fedora_24/x86_64/retroshare06-0.6.1-3.1.x86_64.rpm)  
 - Fedora 23 32bit [v0.6.1-3.1.i686.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/Fedora_23/i686/retroshare06-0.6.1-3.1.i686.rpm)  
 - Fedora 23 64bit [v0.6.1-3.1.x86_64.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/Fedora_23/x86_64/retroshare06-0.6.1-3.1.x86_64.rpm)  
 
For **Fedora 24** run the following as **root**:

       dnf config-manager --add-repo http://download.opensuse.org/repositories/home:AsamK:RetroShare/Fedora_24/home:AsamK:RetroShare.repo
       dnf install retroshare06

For **Fedora 23** run the following as *+root**:

       dnf config-manager --add-repo http://download.opensuse.org/repositories/home:AsamK:RetroShare/Fedora_23/home:AsamK:RetroShare.repo
       dnf install retroshare06
 
###Nightly Builds Fedora
These builds are released daily and may contain contain bugs. 

For **Fedora 24** run the following as **root**:

       dnf config-manager --add-repo http://download.opensuse.org/repositories/home:AsamK:RetroShare/Fedora_24/home:AsamK:RetroShare.repo
       dnf install retroshare06-git

For **Fedora 23** run the following as *+root**:

       dnf config-manager --add-repo http://download.opensuse.org/repositories/home:AsamK:RetroShare/Fedora_23/home:AsamK:RetroShare.repo
       dnf install retroshare06-git
 


##Gentoo
![gentoo logo](../img/install/gentoo_logo.png "Gentoo Install")  

The ebuilds are available [here](https://packages.gentoo.org/packages/net-p2p/retroshare-)


##FreeBSD
![freebsd logo](../img/install/freebsd_logo.png "Freebsd Install")  

Retroshare is currently available on FreeBSD via the ports system.

Link: [freshports](https://www.freshports.org/net-p2p/retroshare)

##Raspberry Pi
![raspberry Pi logo](../img/install/raspberry_pi_logo.png "Raspberry Pi Install")  

At the moment Raspberry Pi builds are planned for the next release to be included. 
Ask the community for handmade builds, or compile it on your own. 
It's easy to follow the Vanilla Debian compile instructions to create 
your own Raspbian binaries. 

##Mageia
![mageia logo](../img/install/mageia_logo.png "Mageia Install")  

Retroshare is currently available on Mageia for i586 and x86_64.  

Sadly the builds are at v0.5.5c and kind of outdated.  
Link: [Mageia](http://mageia.madb.org/package/show/name/retroshare/)  


##CentOS
![centos logo](../img/install/centos_logo.png "CentOS Install")  

###Stable CentOS
Stable builds are official releases.

Stable Package for CentOS:  

 - CentOS 7 64bit [v0.6.1-3.1.x86_64.rpm](http://download.opensuse.org/repositories/home:/AsamK:/RetroShare/CentOS_7/x86_64/retroshare06-0.6.1-3.1.x86_64.rpm)  

For **CentOS 7** run the following as root:  

       cd /etc/yum.repos.d/
       wget http://download.opensuse.org/repositories/home:AsamK:RetroShare/CentOS_7/home:AsamK:RetroShare.repo
       yum install retroshare06

###Nightly Builds CentOS
These builds are released daily and may contain contain bugs. 

For **CentOS 7** run the following as root:  

       cd /etc/yum.repos.d/
       wget http://download.opensuse.org/repositories/home:AsamK:RetroShare/CentOS_7/home:AsamK:RetroShare.repo
       yum install retroshare06-git
