#Compilation

##Compilation on Linux

###Install package dependencies:
#### Debian/Ubuntu
```bash
   sudo apt-get install libglib2.0-dev libupnp-dev qt4-dev-tools \
       libqt4-dev libssl-dev libxss-dev libgnome-keyring-dev libbz2-dev \
       libqt4-opengl-dev libqtmultimediakit1 qtmobility-dev libsqlcipher-dev \
       libspeex-dev libspeexdsp-dev libxslt1-dev libcurl4-openssl-dev \
       libopencv-dev tcl8.5 libmicrohttpd-dev
```
#### openSUSE
```bash
   sudo zypper install gcc-c++ libqt4-devel libgnome-keyring-devel \
       glib2-devel speex-devel libssh-devel protobuf-devel libcurl-devel \
       libxml2-devel libxslt-devel sqlcipher-devel libmicrohttpd-devel \
       opencv-devel speexdsp-devel libupnp-devel libavcodec-devel
```
#### Arch Linux
```bash
   pacman -S base-devel libgnome-keyring libmicrohttpd libupnp libxslt \
       libxss opencv qt4 speex sqlcipher
```

###Checkout the source code
```bash
   mkdir ~/retroshare
   cd ~/retroshare 
   git clone https://github.com/RetroShare/RetroShare.git trunk
```

###Compile
```bash
   cd trunk
   qmake CONFIG+=debug
   make
```

###Install
```bash
   sudo make install
```

The executables produced will be:  
 
 - /usr/bin/RetroShare06  
 - /usr/bin/RetroShare06-nogui  

