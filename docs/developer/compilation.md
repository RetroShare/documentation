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


##Compilation on Windows

###Qt Installation

Install Qt via: [Qt Download](http://www.qt.io/download/)  

Use default options.  
Add to the PATH environment variable

       ;C:\Qt\5.5\mingw492_32\bin;C:\Qt\Tools\mingw492_32\bin;C:\Qt\Tools\mingw492_32\opt\bin  

Depends on wich version of Qt you use.  
Change build-all-mingw32make.bat with these values too if you don't use MSys2.  

###MSYS2 Installation

Choose your MSYS2 installer here: [MSYS2](http://msys2.github.io/)

Follow install procedure.  
Don't forget to sync & Update pacman.  

       pacman --needed -Sy bash pacman pacman-mirrors msys2-runtime  

Restart console  

       pacman -Su  

Install all default programms  

       pacman -S base-devel git mercurial cvs wget p7zip gcc perl ruby python2  

Choose only w64-i686 if you want only compilation in 32b architecture.  

       pacman -S mingw-w64-i686-toolchain mingw-w64-x86_64-toolchain  

###Install other binutils:   
       pacman -S mingw-w64-i686-miniupnpc mingw-w64-x86_64-miniupnpc  
       pacman -S mingw-w64-i686-sqlite3 mingw-w64-x86_64-sqlite3  
       pacman -S mingw-w64-i686-speex mingw-w64-x86_64-speex  
       pacman -S mingw-w64-i686-opencv mingw-w64-x86_64-opencv  
       pacman -S mingw-w64-i686-ffmpeg mingw-w64-x86_64-ffmpeg  
       pacman -S mingw-w64-i686-libmicrohttpd mingw-w64-x86_64-libmicrohttpd  
       pacman -S mingw-w64-i686-libxslt mingw-w64-x86_64-libxslt  

Add MSYS2 to PATH environment variable depends your windows  

       ;C:\msys64\mingw32\bin
       ;C:\msys32\mingw32\bin


###Git Installation

Install Git Gui or other client: [Git Scm](https://git-scm.com/download/win)

Create a new directory named:  

       C:\Development\GIT  

Right-click on it and choose: *Git Bash Here*  

Paste this text on git console:  
git clone https://github.com/RetroShare/RetroShare.git  


###Last Settings


In QtCreator Option Git add its path: *C:\Program Files\Git\bin* 
and select "Pull" with "Rebase"  


Open an MSys2 32|64 shell  
Move to build_scripts:  

       cd /c/Development/GIT/RetroShare/msys2_build_libs/  

###Compile missing library
       make

You can now compile RS into Qt Creator  

For using, and debugging Plugins, you can use [Symlinker](http://amd989.github.io/Symlinker/) to link 
the files in  

       \build-RetroShare-Desktop_Qt_X_Y_Z_MinGW_32bit-Debug\plugins\PluginName\debug\*.dll  
to  
*%appdata%\RetroShare\extensions6*


##Compilation on MacOS

### Qt Installation

Install Qt via: [Qt Download](http://www.qt.io/download/)  

Use default options.  
Add to the PATH environment variable with this temporary solution.  

       export PATH=/users/$USER/Qt/5.5/clang_64/bin:$PATH

Depends on wich version of Qt you use.

###MacPort Installation

Install MacPort and XCode following this guide: [MacPort and XCode](http://guide.macports.org/#installing.xcode)

Start XCode to get it updated and to able C compiler to create executables.  

###Install libraries  

       $sudo port -v selfupdate
       $sudo port install openssl
       $sudo port install miniupnpc
       
For VOIP Plugin: 

       $sudo port install speex-devel
       $sudo port install opencv

Get Your OSX SDK if missing: [MacOSX-SDKs](https://github.com/phracker/MacOSX-SDKs)  

###Last Settings

In QtCreator Option Git add its path:  

       C:\Program Files\Git\bin
       
and select "Pull" with "Rebase"

###Compil missing libraries
####SQLCipher
       
       cd <your development directory>
       git clone https://github.com/sqlcipher/sqlcipher.git
       cd sqlcipher
       ./configure --enable-tempstore=yes CFLAGS="-DSQLITE_HAS_CODEC" LDFLAGS="-lcrypto"
       make 
       sudo make install

NOTE, might be necessary to *chmod 000 /usr/local/ssl* temporarily during *./configure* if 
homebrew uses newer, non-stock ssl dependencies found there. configure might get confused.

####libMicroHTTPD
The one with port don't have good support.

       cd <your development directory>
       wget http://ftpmirror.gnu.org/libmicrohttpd/libmicrohttpd-0.9.46.tar.gz
       tar zxvf libmicrohttpd-0.9.46.tar.gz
       cd libmicrohttpd-0.9.46
       bash ./configure
       sudo make install

You can now compile RS into Qt Creator or with terminal

       cd <your development directory>
       git clone https://github.com/RetroShare/RetroShare.git retroshare
       cd retroshare
       qmake; make

You can find compiled application on *./retroshare/retroshare-gui/src/RetroShare06.app*
