---
title: Test
date: 2016-12-27 03:00:01
tags:
---

## Before starting

We will use the [firmata][1] protocol to talk with the microcontroller.

Firmata is a protocol based on midi that provide an "API" to control your MCU hardware.

In the examples and exercices that you will find here, we will use Javascript, nodejs, and the [Johnny-Five][2] package

You will need [nodejs][3] (somehow recent) to use the test tool and the workshoper 

## Test firmata on the board

the board should be flashed with firmata but let's try anyway

in a terminal and in your project directory

```
git clone git@github.com:catbotFactory/yldWorkshop.git
cd yldWorkshop
npm install
npm run firmTest
```

firmTest should say something like 
```
your board is ready to use !
```
and exit.

If not go [here][4] and come back

## Test and Calibration

```
npm run cal
```

Will ask you a few question and help you calibrate your catbot.  
Once done it will write a ```~/.catbotrc``` file that will be loaded by the catbot lib, allowing you simple override of the default options.  
if you have an analog joystick you can enable it in this file.

you are now ready to play with your catbot go [here][5] 

[1]:https://github.com/firmata/protocol
[2]:https://johnny-five.io
[3]:https://nodejs.org/en/
[4]:/troubleshooting#Firmata
[5]:/lasercat
