pyazo
=====

Gyazo and Gifzo compatible server by perl


Wait a moment ...
====
[Pyazo2](https://github.com/uzulla/Pyazo2) was released.


pyazo(THIS) is very simple, usuable. it will no longer develop.

[Pyazo2](https://github.com/uzulla/Pyazo2)  is new version of pyazo. 
Amon2 based.
new feature (auto resize, auto JPEG orientation correction, more smart html).


install and run
====

```
cpanm --installdeps . 
vi start.sh # if you use Gifzo compatible.
start.sh 
```

how to use with Mac gyazo client
================================
please edit ```Gyazo.app/Contents/MacOS/Gyazo```

```
HOST = 'yairc.cfe.jp'
CGI = '/'
UA   = 'Gyazo/1.0'
```
and

```
Net::HTTP.start(HOST,5000){|http|
```

(Huh? Windows? I dont know...)


Gifzo compatible is optional.
====

If you want use Gifzo compatible, You must install ffmpeg and gifsicle or (ImageMagick( or YoyaMagick)).


start.sh options
====
- export FFMPEG_PATH="/usr/bin/ffmpeg"

FFMpeg path. require by gifzo compatible

- export IM_CONVERT_PATH="/usr/bin/convert"

ImageMagick(or yoya magick or compatible) convert command path. require by gifzo compatible

- export GIFSICLE_PATH="/path/to/gifsicle"

path to gifsicle. require by gifzo compatible

http://www.lcdf.org/gifsicle/

gifsicle is REALLY fast, RECOMMEND

- export FORCE_TMP_GIF="yes"

use GIF temprary file format, fast and compact filesize.(but bit lower quality)

(force yes when use gifsicle)


Sample
====

pyazo is using in Yancha
http://yancha.hachiojipm.org/


rapid setup on instantserver.io (written in japanese)
http://uzulla.hateblo.jp/entry/2013/06/19/202650


see also
====

Gyazo
http://gyazo.com/ja

Gifzo
http://gifzo.net/
