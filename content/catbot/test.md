---
title: Test
layout: Page
hero: /assets/catHero.svg
# hero credit: https://www.flickr.com/photos/pslee999/15589950511/
#cta:
#  label: About this theme
#  link: "about"
---

## Before starting

We will use the [firmata][1] protocol to talk with the microcontroller.

Firmata is a protocol that provide an "API" to control your MCU hardware.

In the examples and exercices that you will find here, we will use Javascript, nodejs, and the [Johnny-Five][2] package

You will need [nodejs][3] (somehow recent) to use the test tool and the workshoper 

## Test / Install firmata on the board

the board may be flashed with firmata, let's check (if the board is sealed, it isn't)

in a terminal and in your project directory (if you have any)

```
git clone git@github.com:catsAndSolenoids/yldWorkshop.git
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
[4]:/catbot/troubleshooting#Firmata
[5]:/catbot/lasercat
