# DeviceDriver-robosys2018

# Overview
端末でRaspberry Pi3 Model B+上の2色のLEDを操作。

# Description
端末でRaspberry Pi3 Model B+上の2色のLEDを操作。

# Demo
https://youtu.be/ZaO6G3mgpqE

# Requirement
* Computer
  * Raspberry Pi3 Model B+
* OS
  * Raspbian

# Install
```
$ git clone https://github.com/Yu0097/DeviceDriver-robosys2018.git
```

# Usage
```
$ make
$ sudo insmod ledchika.ko
$ sudo mknod /dev/ledchika0 c 243 0
$ sudo chmod 666 /dev/ledchika0
```

LEDの点灯
```
$ echo [r or g] > /dev/ledchika0
```
LEDの消灯
```
$ echo [R or G] > /dev/ledchika0
```

# License
MIT License
