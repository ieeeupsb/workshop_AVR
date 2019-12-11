Exercise 6: IR Remote

In this exercise we hope to teach you how to use an IR remote. As seen in the slides, the remote control sends an RC5 signal to the receptor. As you don't have any oscilloscope here, the command part of the signal sent by the remote (that identifies the button being pressed) will be given for some buttons.

The PIN 1 of the receptor should be connected to the GND, the PIN 3 to Vcc and the PIN 4 to INT0/PD2.

if(((cmdnum) == 51)) (on/off button)
if(((cmdnum) == 50)) (mute button)

if((cmdnum) == 47)  (sound +)
if((cmdnum) == 46)  (sound -)
if((cmdnum) == 31)  (channel +)
if((cmdnum) == 31)  (channel -)           