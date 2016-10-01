# Standard Plugins
The following plugins are generally part of downloaded/installed packages and are included with the standard source code downloads. You may need to download and install additional development libraries to compile.

## VOIP

VOIP provides video and voice communications with other friends who have the facilities. 

To compile and use (for Gnu/Linux):

    cd [your retroshare source folder]/plugins/VOIP
    qmake && make clean && make
    cp lib*.so ~/.retroshare/extensions6

Restart RetroShare, enabling the plugin when asked. You can change settings in Options->VOIP.

## FeedReader

FeedReader acts as an RSS feed collector for RetroShare, gathering selected news feeds into RetroShare.

To compile and use (for Gnu/Linux):

    cd [your retroshare source folder]/plugins/VOIP
    qmake && make clean && make
    cp lib*.so ~/.retroshare/extensions6

Restart RetroShare, enabling the plugin when asked. You can change settings in Options->FeedReader.


# Additional Plugins
## FriendMap
Displays a globe, with location of friends on it.

Under active development, works with 0.6.0 and Qt5, from <https://github.com/chozabu/FriendMap>

## Lua4RS
Allows Lua scripts to run under RetroShare for various administrative tasks.

Works with 0.6.0 and Qt5, from <https://github.com/sehraf/Lua4RS>.

## RetroChess
Play one game of chess against another player.

Developmental and may have bugs.

Under development, please report any issues on github page, from <https://github.com/chozabu/RetroChess>.
