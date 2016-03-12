---
title: "Practice #22: Mission Planner and Ultrasonic"
date: 2016-02-27
layout: post
categories: jekyll update
---

{% include image.html
            img="http://i.imgur.com/tT6Q8Ai.jpg"
            title="title for image"
            caption="Testing of the Ultrasonic Sensor"
            width="266px"
            height="473px"
%}


## Updates

* A SEDS@UCSD friend helps our team and begins printing 

## Daily Objectives

Today’s focus is to advance our progress in sending Navio+ outputs and recieving
inputs. Our primary objective is to be able to use the RPI2 to send signals
through the Navio+ to drive a servo by the end of practice. This will require
learning about RC calibration. Our secondary objective is to have RTK and APM
Rover Navio+ Drivers installed on the second RPI2. We also need to familiarize
ourselves with using Lidar and test its outputs. Our third daily objective is,
if RTK installs quickly, to read ultrasonic inputs through the Navio+ into the
RPI2 shell/command line. Our fourth objective is create a chassis maintenance
guide. We should also be proactive and look for other 3D printing alternatives.
Finally, we will spend time today covering communication logistics.

## Progress Reflection

**Peripherals**

* Today Alexander and Alec learned that autopilot functionality on the Navio+ is
  done through a GCS (ground control station) like MissionPlanner or APM
Planner. Both of these software require setting up RC controls before any
autopilot functionality can be configured. This means that before any outputs
can be sent from the Navio+, the RC system needs to be connected to the Navio+
and used to calibrate a GCS. Alexander and Alec had trouble connecting the
HK-TR6A V2 receiver to the Navio+. This turns out to be because the receiver
sends only PWM outputs but the Navio+ RC input port is labeled "PPM". The two
are incompatible so our next best option is to get a PWM to PPM SBUS connector.

* Jeffry and Sanil tested the ultrasonic sensors. They found two issues. 1) The
  sensor can't tell difference from 0 to ~1ft. 2) The sensor will have to be
positioned in certain way to be useful. Also note that blowing on the sensor
does not change voltage when tested on o-scope (as opposed to a handheld
multimeter). They also found how to connect ultrasonic analog to the RPI2 by
using the Navio+’s ADC and it will require surface mount soldering. To use both
ultrasonic sensors we need might need another [ADC](http://www.ti.com/lit/ds/symlink/ads1115.pdf) or need to join the sensors.

* Wilfred has RTK installed on the second RPI2 and is able to live calibrate the
  Navio+ through the APM Planner 3.0 software on his computer.

**Hardware**

* Sanil found available 3D printing at the [La Jolla Public Library.](http://www.lajollalibrary.org/your-library/facilities/) He also started a
chassis maintenance guide so that team members know how to keep a functioning
chassis.

**Documentation**

* Karina updated our logo. She started by removing the scattered five icons,
  then incorporating the IEEE logo into our logo, then making our own logo. We
still need to decide on our team name.

* Karina made a Cloud9 & GitHub account. Alex introduced Karina to posting on
  our webpage and she made a mock practice #22 post to the website. 
 
**Logistics**

* We are finished preparing for our project, have necessary materials, and can
  effectively organize as a team. At this time, our project has has progressed
to a state time-dependant testing and technical work so Alec emphasized the
importance of arriving to practice on time and reacting to Slack notifications
within 24hrs.

* The importance of sharing information and work through Google Drive, Trello,
  and Slack is reiterated.

* Everyone recorded their shirt size in preparation to get team T-shirts.

Attendance: Alec, Alex, Alexander, Jeffry, Karina, Sanil, Wilfred

\-  Alec Guthrie (February 28, 2016)
