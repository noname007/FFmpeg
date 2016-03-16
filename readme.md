

## 安装sdl1.2 否则无法编译出来ffplay



 sudo apt-get install libsdl1.2-dev libsdl-image1.2-dev libsdl-mixer1.2-dev libsdl-ttf2.0-dev libsdl-gfx1.2-dev

## 安装x265编码库
sudo apt-get install libx265-dev

## 编译ffmpeg

安装过程如果缺少包，就安装，如安装 lib×-dev 等包
~~`./configure --enable-gpl --enable-libass --enable-libfdk-aac --enable-libfreetype --enable-libmp3lame --enable-libopus --enable-libtheora --enable-libvorbis --enable-libvpx --enable-libx264 --enable-libx265 --enable-nonfree --pkg-config-flags="--static"` [^1]~~
~~ ./configure  --enable-gpl --enable-libass --enable-libfdk-aac --enable-libfreetype --enable-libmp3lame --enable-libopus --enable-libtheora --enable-libvorbis --enable-libvpx --enable-libx264 --enable-libx265  --enable-nonfree  --enable-shared ~~

./configure  --enable-gpl --enable-libass --enable-libfdk-aac --enable-libfreetype --enable-libmp3lame --enable-libopus --enable-libtheora --enable-libvorbis --enable-libvpx --enable-libx264 --enable-libx265  --enable-nonfree   --enable-shared  --prefix=/usr/

~~./configure --enable-gpl --enable-libx265~~

sudo make



sudo make install


[^1]:
     http://trac.ffmpeg.org/wiki/CompilationGuide/Ubuntu


