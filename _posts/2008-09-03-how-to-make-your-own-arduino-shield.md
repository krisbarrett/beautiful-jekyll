---
layout: post
title:  "How to Make Your Own Arduino Shield"
date:   2008-09-03 12:00:00
categories: ['blog']
bigimg: '/img/arduino_shield.jpg'
---
After many months of working on my Arduino based project, I decided to finalize my project by making my own custom PCB.  At first I wanted to design a PCB that connected to the Arduino through a series of cables.  After some thought however, I realized that a shield would be better because it would eliminate the need for cables.  This tutorial assumes an understanding of Cadsoft Eagle.  For more information about Eagle, see the Eagle Tutorials section below.  Here are the steps to make your own Arduino shield:

1. **Part Selection** - Carefully select your parts. Ensure that your parts meet your performance and power requirements.  It is better to carefully choose your parts now, than wish you chose something else later.

2. **Prototype** – Prototype your design on a breadboard.  Ensure that your functional, performance, and power requirements are being met.  Change your design as necessary.  Do not begin designing the PCB until you are completely satisfied with your prototype.

3. **Schematic Capture**

   a. **Add Custom Parts to Eagle** – Place all of your parts in the schematic before drawing any wires.  This allows you to identify which parts you will need to create yourself.  I had to create a custom part for the Arduino.  Drawing a symbol for the Arduino was easy.  Drawing the package was a little bit more difficult because I had to determine the spacing between the headers.  I easily obtained this information from the Arduino Eagle files which I downloaded from the Arduino website.  Download my Eagle Arduino library [here](/downloads/arduino.lbr).

   b. **Connect Parts** - After placing all of your parts in the schematic, carefully connect your parts together using the wire tool.  If you make a mistake on your schematic, it will ultimately show up on your PCB.

4. **PCB Layout** - Place the parts on the board.  If your PCB is long enough, the PCB will rest on top of the USB connector on the Arduino.  Parts and traces should not be placed here because it could potentially short out your PCB.  I accidentally placed the DC power connector in this area. Fortunately,  I was able to insulate the USB connector with a piece of electrical tape.  Also, follow PCB layout guidelines.  I learned this the hard way when I discovered that the rapid switching of the transistors was inducing a voltage in one of the traces connected to the button.

5. **PCB Fabrication** – Generate the CAM files.  You could fabricate the PCB yourself, but I highly recommend BatchPCB.  BatchPCB fabricates inexpensive, production quality PCBs.  The only drawback is that you have to wait three weeks to a month to receive your order.  BatchPCB has a tutorial on generating the files that they need to fabricate your PCB.

## Final Thoughts
Although I am not happy with the way my PCB turned out, I learned valuable information about PCB design.  I am sure that if I follow PCB layout guidelines, I can get this PCB to work properly.  I hope people can learn from my mistakes on this project and design a better Arduino shield of their own.

## Eagle Tutorials
* [Schematic Capture](http://www.sparkfun.com/commerce/tutorial_info.php?tutorials_id=57&sipp=1&page=8)
* [Creating Custom Parts](http://www.sparkfun.com/commerce/tutorial_info.php?tutorials_id=57&sipp=1&page=10)
* [PCB Layout](http://www.sparkfun.com/commerce/tutorial_info.php?tutorials_id=57&sipp=1&page=9)
* [Generating CAM Files](http://www.batchpcb.com/eagle-tutorial.php?osCsid=6fafc3f166d30af2bc9598efd0d9c71f)
