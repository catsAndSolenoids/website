---
title: Troubleshooting
layout: Page
hero: /assets/catHero.svg
# hero credit: https://www.flickr.com/photos/pslee999/15589950511/
#cta:
#  label: About this theme
#  link: "about"
---

# Troubleshooting

Here we will see the possible problem you may encounter, and their possible solutions

## How to install Firmata
to install firmata on your  board, you can use [firmata-party][1]
plug the arduino to your computer

```
npm install -g firmata-party
firmata-party uno
```
DONE

you can also use the arduino IDE 

- [Download arduino IDE][2]
- Plug the funduino in a usb port
- Open the funduino IDE. Ensure that you selected your funduino type (arduino uno)and port
- Open Files > Examples > Firmata > StandardFirmata
- Upload it (the button with an arrow in the IDE or File > Upload).

## when I move the servo the  app crashes
if your board crashes when you try to move the servo they are most likely underpowered

- check that your funduino is connected to the 9v psu
- check that the switch on the funduino is set to 5v

## This list is short! My problem is not here!

if you can'f find solution to your issue, fill one [here][3]

[1]: https://github.com/noopkat/firmata-party
[2]: https://www.arduino.cc/en/Main/Software
[3]: https://github.com/catbotFactory/yldWorkshop/issues
