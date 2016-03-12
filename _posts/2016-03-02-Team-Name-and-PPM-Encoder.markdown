---
title: "Practice #23: Team Name and PPM Encoder"
date: 2016-03-05
layout: post
categories: jekyll update
---

{% include image.html
            img="http://i.imgur.com/ERKV6kK.jpg"
            title="title for image"
            caption="Team Logo with new Team Name"
%}


## Updates

* Sent in more reimbursement requests for Alec and Wilfred
* Ordered a 3DR PPM encoder
* Friend's 3D printer jammed while printing our stuff :( we need an alternative
  printing resource


## Daily Objectives

At the beginning we will choose our team name, finalizing the logo and T-shirts,
and talk about fundraising. With logistics out of the way, our 23rd practice
will focus on connecting sensors and reading their data. Our first objective is
to test the Lidar by reading inputs to the computer through USB, and then to
RPI2 through USB or serial. Next we will solder header pins onto one of the
RPI2's ADC, connect the ultrasonic sensor, and digitally read the converted
analog inputs to the RPI2 or MissionPlanner. Lastly, if we have time the Chassis
Maintenance Guide should be updated.

## Progress Reflection

**Peripherals**

* Wires were soldered onto AIN2 and AIN3 on the analog to digital converter. The
  other two pins available must then be tied to the GPIO ports to the
microcontroller. The communication protocol is I2C

* Downloaded Terminal Software to test Lidar readings on computer. Got
  successful readings to output onto computer. Used the sensor manual to help
get the readings and set up the Lidar.

* Without a PWM-PPM encoder, not much work could be done with MissionPlanner’s
  Radio Control Calibration. Alexander helped teach Alec to connect the Navio+
to MissionPlanner on his computer and view live sensor testing.

**Funding**

* Determined future dates for fundraising at DLush: March 31st & April 9th

* Future fundraising idea: Santorini

**Documentation**

* Documentation Sub Team stuff about team logo, shirt, and name
 
* Waiting on confirmation of team name

Attendance: Alec, Alex, Alexander, Christian, Jeffry, Karina, Sanil, Wilfred

\-Alec Guthrie & Alex Hermstad (March 03, 2016)
