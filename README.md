# DeviceDriver-robosys2018

# Overview
Raspberry Pi3 Model B+上の2色のLEDでLチカを行う。

# Description
端末でRaspberry Pi3 Model B+上の2色のLEDを操作。

# Demo
https://youtu.be/0Pk_HCv-g8I

# Requirement
* Computer
   * Raspberry Pi3 Model B+
* OS
   * Raspbian* p
* Parts
   * Red LED
   * Green LED
   * Bread Board
   * Jumper Wire (male - female)
   * Carbon Resistor

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
GNU General Public License v3.0
