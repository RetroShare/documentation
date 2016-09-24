RetroShare is available for various Operating Systems. 

##Ubuntu
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

Retroshare is currently available on Debian Stretch for i386 and amd64 architectures.  
You can download packages from GitHub released by the Development Team: [Debian packages](https://github.com/RetroShare/RetroShare/releases/)  

Stable and Nightly Builds are also available here:  
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

Retroshare is currently available on openSUSE.

Install stable release via: [Yast oneclick]()

Link: [13.2](http://software.opensuse.org/ymp/home:AsamK:RetroShare/openSUSE_13.2/retroshare06.ymp)    [13.1](http://software.opensuse.org/ymp/home:AsamK:RetroShare/openSUSE_13.1/retroshare06.ymp)    [Factory](http://software.opensuse.org/ymp/home:AsamK:RetroShare/openSUSE_Factory/retroshare06.ymp)

Download binary or add Repository manually:  
[Stable release](https://software.opensuse.org/download.html?project=home%3AAsamK%3ARetroShare&package=retroshare06)    [Nightly snapshot](https://software.opensuse.org/download.html?project=home%3AAsamK%3ARetroShare&package=retroshare06-git)
