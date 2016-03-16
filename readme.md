

## 安装sdl1.2 否则无法编译出来ffplay



 sudo apt-get install libsdl1.2-dev libsdl-image1.2-dev libsdl-mixer1.2-dev libsdl-ttf2.0-dev libsdl-gfx1.2-dev

## 安装x265编码库
sudo apt-get install libx265-dev

## 编译ffmpeg

./configure --enable-gpl --enable-libx265

sudo make

sudo make install
