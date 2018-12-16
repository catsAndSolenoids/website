---
title: Connect
layout: post
hero: /assets/catHero.svg
---

## Before starting
Let's have a look at our Funduino (the Arduino clone this kit uses)

![funduino details](/assets/connect/funduino_01.png)


- 1 : USB connector, allow serial connection and power up the board for small project
- 2 : Voltage switch, change boards and pin voltage (3V3 or 5V) (put yours to 5V)
- 3 : Power in, barrel (circular) connector you plug the 9v PSU here, needed for the servo motors to run
- 4 : D13 led, onboard led, linked to pin 13, if you set this pin to HIGH, the led lights up, it also blink during firmata initialisations
- 5 : digital pins row, 14 (0-13) contollable digital (1 or 0) pin
- 6 : Vout pins row, 14 pin providing 3V3 or 5V depending on board conf
- 7 : Ground pins row, 14 pin to the gnd
- 8 : analog pins row, 6 contollable analog (0 to 1023) pin

Unplug the funduino from usb and / or power before connecting anything.
Then check that the voltage switch (2) is set to 5V (servomotors need 5V)

## Catbot
![Catbot wiring](/assets/connect/funduino_02.png)

### laser
the laser has 3 pins, but the middle one does not do anything (it's cheaper to
manufacture this way), so the outer two pins from the laser itself connect to the red
and blue wires, they later connect to other colors, we will call the blue one (-) and the red one (+). connect the blue (-) wire to the pin 13 in the ground (7) row (blue row)
then connect the signal wire to pin 12 in the signal (5) row (yellow one)

###  Y axis servo
the Y axis is the servo motor on the top part, linked to the laser.
the servo have a connector at the end of the wire the collored wire are

- brown : ground wire => blue row
- red : Vin wire => red row
- orange : signal wire => yellow row

place the connector on the D11 col, jumping one col after the laser one.

### X axis servo
Same as Y but on D10 the row befor the X one.

Your catbot is build and wired.

## Joystick

The joystick uses five wires, on the left side of the joystick you have 5 pins 
with labels on the side, connect one side of the strip to them and the other side to the board like in the picture bellow:

![Catbot wiring](/assets/connect/funduino_03.png)


- GND : ground, connect it to any pin in the blue rows ('ground' section)
- +5V : VIN, connect it to any of the red row (+5V)
- SW : Joystick switch, this one will go on the signal row 9 (the one close to the servos) separate the wire from the main strip to get some room
- VRx : X axis, potentiometer for the X axis connect to the pin labeled 'VRx' in the picture (A0)
- VRy : Y axis, potentiometer for the Y axis connect to the pin labeled 'VRy' in the picture (A1)

## Next step
Go to calibrate your bot [here][1]

you will have some leftover bit, some plastic horn for the servo motors, and some screws.

screws can be used later on, when the catbot is calibrated to keep the servo and the turret in place, to do so use a small screwdriver to screw them un the middle of the servo gear through the horn

[1]:/catbot/test
