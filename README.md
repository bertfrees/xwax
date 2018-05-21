# xwax-pideck

This branch contains the 64 Studio patches for xwax for use with Pideck

How to build on Debian sid:

install build dependencies:
```
sudo apt-get install build-essential libasound2-dev libjack-dev libsdl-ttf2.0-dev
sudo apt-get install fonts-dejavu-extra cdparanoia ffmpeg mpg123
```

build:
```
./configure --prefix /usr --enable-alsa --enable-jack
make clean
make
```

run (you may need to change the -a argument):
```
./xwax -q 0 -i import -s scan -a hw:2,0 -g 800x430 -l ~/Music
```
