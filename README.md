Note di L.Fini 4/11/2019

Il software è stato compilato e provato con una scheda:

Arduino/Genuino Zero (Native USB port)

- Risponde al ping
- Risponde alla URL: http://192.168.0.67

--------------------------------------
Le note seguenti sono quelle originali

# OnStepEthernetServer

This is the Arduino webserver for OnStep.  It provides Ethernet
(IP) access to connect to OnStep via command channel and/or website.
This works with Sky Safari (tablets/phones,) my OnStep Android App,
and my ASCOM driver (PC.)

For my testing I used an Arduino M0 and Arduino Ethernet Shield R3
(W5100.)  Other configurations are untested but Arduino's with ARM MCU's
and similar Ethernet Shields should generally work.  There are reports
of the Arduino Ethernet Shield V2 not working with the M0 so aviod that!

Use the Arduino IDE's "Tools->Boards->Boards Manager" menu to add ARM
device support.

Download the OnStepEthernetServer.zip file from GitHub.

Unzip the folder inside and rename it to "OnStepEthernetServer". This
can be on your desktop or in your ~/Documents/Arduino folder.

Open the OnStepEthernetServer.ino file inside this folder.  Find the
"Config.h" tab and make any changes as required for your setup.  Upload.


Once the firmware is on the device simply connect the serial interface
lines to OnStep's Serial1 port similar to how a Bluetooth module would
be connected.

The Teensy3.2 and Launchpad TM4C OnSteps are best for this but the
Mega2560 should work too (probably.)

