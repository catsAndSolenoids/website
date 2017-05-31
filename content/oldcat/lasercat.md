---
title: Lasercat
date: 2016-12-26 03:22:03
tags:
---

## lasercatWorkshop

if you are not familiar with nodebots or arduinos, you shoud start by doing the [lasercat workshop][1] that we made with [Tableflip][2] for LXJS 2014

if you cloned the yld-workshop repo, you have the boilerplate code for the lasercat exercise in the exercises folder, fork the repo and start from there.

## Johnny five

Johnny five is a JavaScript Robotics & IoT Platform and is used by the catbot module

interesting APIs for the cat are 

- [LED][5] for the laser
- [Servo][6] to move the turret
- [Joystick][7] to use the joystick if your kit have one.

## What's next ?

it is a bit up to you from here on

- there is a library to play with the bot on npm ```npm i catbot``` details [here][4]
- if you have some electronic component (like a beginer arduino kit) around, you can also do the [nodebot-workshop][3]

[1]: https://github.com/tableflip/lasercat-workshop
[2]: https://tableflip.io/
[3]: https://github.com/tableflip/nodebot-workshop
[4]: https://github.com/gorhgorh/catbot
[5]: http://johnny-five.io/api/led/
[6]: http://johnny-five.io/api/servo/
[7]: http://johnny-five.io/api/joystick/
