# ECE 362 Group Project
Make an Etch a Sketch (with an stm32)!

## A brief description of our project and what it will be able to do:

An etch a sketch with two knobs (potentiometers) that will record motion to a LCD screen allowing the drawing of images. Additionally using an accelerometer the user will be able to shake the screen and reset their drawing

 - An ability to display graphics on the TFT display using SPI protocol and external interface
 - An ability to receive and translate analog directional information using the internal ADC peripheral
 - An ability to use internal timers to control display and game flow in real time
 - An ability to use an external I2C accelerometer to interrupt and clear the screen

## Main features of our project:
Our etch-a-sketch will have 3 external components: the TFT LCD display, the two potentiometers, and an I2C Accelerometer, and 2 potentiometers for X and Y control.

The TFT LCD display and potentiometers are already in our lab kits, although we may procure better potentiometers from the ECE shop which has a drawer full. We also plan on using an I2C accelerometer to shake the board and clear the screen. For this, we would like to use https://www.adafruit.com/product/2019?gad_source=1&gclid=Cj0KCQjwu-63BhC9ARIsAMMTLXQVQhPq4wVcWrk7dFT_t-0NDRVO2zZFT1a4A0YmWToC_e04hHX0ia0aAqd-EALw_wcB
which we will purchase when our project has been approved (or find an alternative I2C accelerometer in the ECE shop if they have one).


## Eternal interface formats our project will use:
Our system will take in input from 2 different external sources: a potentiometer/knobs/joysticks, and an accelerometer. These parts should be readily available in the ECE shop or cheap to purchase. We will choose whatever is optimal for the constraints of this project without needing to purchase extra parts. 
These external parts will utilize the following formats:
 - SPI for display
 - Analog for input of knobs
 - I2C for accelerometer

## Internal peripheral subsystems our project will use:
The 4 internal peripheral subsystems that our project is gonna use are:
 - At least 1 timer for updating the display and 1 timer for triggering DMA request
 - An ADC for the x-axis and y-axis knobs
 - a DMA for the ADCs
 - An SPI for the display system for the etch-a-sketch.

## Planned timeline for completing the various steps of our project:

Week 9: Submission DEADLINE (10/14)
Schematic complete 10/21
Pseudocode complete 10/21
Week 10: Breadboard Practical
Breadboard Done 10/26
Initial Code Complete 11/2
1 week to debug
Final integration complete 11/9
1 week to buffer
Project works by 11/16
Week 14: Demo DEADLINE (11/22)


## Related published projects, products, or articles that you found that are similar to our project:

There was one previous ECE 362 mini-project that implemented an etch-a-sketch, the video showing the final product is below:
https://www.youtube.com/watch?app=desktop&v=kgjA8iDKNtA
While this is a good example of a successful implementation of this project, ours will have some differences. They are best described through the following points:
 - Different display: LCD rather than an LED matrix (greater resolution)
 - Different physical implementation
