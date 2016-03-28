---
title: "Practice #19: Working with Motor and RC Input"
date: 2016-02-17
layout: post
categories: jekyll update
---

{% include image.html
            img="http://i.imgur.com/Qr4n5xD.jpg"
            title="title for image"
            caption="Alec and Alexander Working to Power Navio+"
            width="360px"
            height="592px"
%}

## Updates

- New orders: Alec and Wilfred planned to finish the chassis with the discovered
  motor pinion gear but that gear’s teeth didn’t match the chassis spur gear.
Their “pitches” were different so Wilfred ordered another 5mm, 48pitch, 20tooth
pinion gear.

- Building: Alec and Wilfred finished connecting basic power distribution. They
  had to fix the mismatching (male-male, female-female) XT60 connections by
resoldering the BECs and making a male-male adapter. This took them two tries…

- New Parts: The correct pinion gear arrived!

- Website: Old practice backlogs have been made live on the website.`

## Daily Objectives

Today’s goal was to continue progressing through our winter quarter timeline.
Specifically we set out to attach the motor and mount the battery, program the
RC controller transmitter and ESC, and send RPI2 commands to the Navio+ servo
rail outputs and link those with GPS signals using mission planner.

## Progress Reflection

We were only able to complete 1/3 of our initial daily objectives.

**Peripherals**

* Christian followed the ESC instruction manual for using the LCD Program Box to
  program the ESC and its outputs to the motor. He identified 3 functions of the
Program Box - program ESC settings via LCD screen, USB adapter to PC using
firmware, Lipo battery voltmeter. Here is how he established a connection to the
program box:
   * Insert white,red,black program wire from ESC to LCD Program Box
   *  Turn on ESC via switch WITHOUT holding on Set Button.
   * After a few seconds, green flash and beep. Then, flashing red.
   * Press any button to connect LCD Program Box.
   How to Use Program box:
   * Press Item to cycle through settings.
   * Press Value to cycle through preset programmable values.
   * Press R/P to see Software Version.
   * Press OK to save changes.

* Christian checked the ESC software version to be:  105_150480 and then
updated the LCD Program Box firmware to version HW310_V2.1. Lastly, he
successfully tested out the lipo battery voltmeter on the ECO Power 30C battery
by inserting the program wire of the battery (red, black, black) into "Battery
Check" pins of LCD Program Box.

* Alexander and Alex researched how to use the Radio Transmitter to interface
  with the APM Planner. Alexander and Alex are still in the progress of getting
a successful signal from the transmitter to the screen on the Mission Planner.
They worked with the documentation on the APM Rover site which describes a first
time setup requiring the RC Transmitter to be connected as well as using
documentation page for the [RC Input for navio+](http://docs.emlid.com/navio/Navio-dev/rc-input/).
 More research needs to be done,
but it might be possible that we need a decoder for the signal as described in
the Erle-Brain 2 page with [this picture](http://erlerobotics.com/docs/img/Robots/common_parts/ppmencoder_connection.png).
There are also [specific instructions for the
Erle-Brain](http://rover.ardupilot.com/wiki/common-compatible-rc-transmitter-and-receiver-systems-erle-brain-2/), which is similar to the
Navio+.
  

**Hardware**

* Jeffry installed the pinion gear to the spur gear and mounted the motor so the
  wires were accessible.

Attendance: Alec, Alex, Alexander, Chris, Jeffry


\- Alex Hermstad & Alec Guthrie (February 22, 2016)
