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

Firmata is a protocol based on midi that provide an "API" to control your MCU hardware.

In the examples and exercices that you will find here, we will use Javascript, nodejs, and the [Johnny-Five][2] package

You will need [nodejs][3] (use 6 or 7, or the version you have if it is more than 3) to use the test tool and the workshoper, if you don't have node installed on your computer and don't know how to install it, please ask any of us, we will help you.

## Test firmata on the board

the board should be flashed with firmata but let's try anyway

in a terminal and in your project directory

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

If not (if the pack for the board is closed) go [here][4] and come back

You are now ready to play with your catbot go [here][5] 

[1]:https://github.com/firmata/protocol
[2]:https://johnny-five.io
[3]:https://nodejs.org/en/
[4]:/catbot/troubleshooting#Firmata
[5]:/catbot/lasercat
