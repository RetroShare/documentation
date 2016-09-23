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
