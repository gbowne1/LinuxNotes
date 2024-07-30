# Connecting to twitch.tv using mpv

## Debian install

The following packages need to be installed

youtube-dl
yt-dlp
vapoursynth-python3
samba-libs
rtmpdump
python3-websockets
python3-tk-dbg
python3-pycryptodome
python3-pyxattr-dbg
python3-pyxattr
python3-gdbm-dbg
python3-dbg
python3-brotli
python3.7-dbg
python-talloc
python-pyxattr-doc
phantomjs
netselect-apt
netselect
mplayer-doc
mplayer
mpv
libzimg2
libvorbisidec1
libvapoursynth-script0
libvapoursynth
libtevent0
libtesseract4
libsmbclient
libpython3.7-dbg
libpython3-dbg
liblept5
libldb1
libfribidi-bin
libenca0
libdirectfb-extra
libdirectfb-1.7-7
fping
bidiv
mpv

this should be the complete dependency tree for mpv to work properly on debian based systems and maybe Ubuntu and others.

## starting mpv

to connect to twitch.tv use the https://twitch.tv/ full link for any channel you want to watch.

the command syntax is `mpv https://twitch.tv/channelnamehere`

## notes

You won't get Twitch chat. It will start with an ad playing with a countdown.

If you know of any other dependency that needs to be installed please let me know.

you may not need youtube-dl as its deprecated but wouldn't hurt to have installed as wel as it may come up in suggested packages.

you will need IRC client to connect to twitch chat..  I may make a guide for rtmp streams or network streams. but it should be pretty much the same.
