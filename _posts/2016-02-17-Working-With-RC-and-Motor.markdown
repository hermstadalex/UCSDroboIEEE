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

   Christian checked the ESC software version to be:  105_150480 and then
updated the LCD Program Box firmware to version HW310_V2.1. Lastly, he
successfully tested out the lipo battery voltmeter on the ECO Power 30C battery
by inserting the program wire of the battery (red, black, black) into "Battery
Check" pins of LCD Program Box.

* Alec tried to program the RC controller using the IEEE Quadcopter Project’s
  PL2303 USB-TTL adapter. He mostly referenced the RC system instruction manual
and this hobbyist's blog suggested by Ian. Alec installed the programming
application T6config.exe, connected the dongle, and started the application.
While starting the application throws a warning "Invalid Port Number” and once
running the Serial Settings option does not show any available COM ports. Alec
also noticed that the device driver didn’t work and the Windows10 Device Manager
throws the error "This device cannot start. (Code 10).” Alec attempted to fix
the errors by installing community drivers and the official
PL2303_Prolific_DriverInstaller_v1_12_0 from Prolific's website, but the
problems were unresolved and the RC controller remained unprogrammed.

Attendance: Alec, Alex, Alexander, Chris, Jeffry


\- Alec Guthrie (February 6, 2016)
