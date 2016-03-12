---
title: "Practice #21: Testing Ultrasonic Sensors and Connecting Servo"
date: 2016-02-24
layout: post
categories: jekyll update
---

{% include image.html
            img="http://i.imgur.com/BBoI9MM.jpg"
            title="title for image"
            caption="Wilfred, Christian, and Jeffry Working on the Multifunction
            LCD Programming Box."
%}


## Updates

* We implemented a list of planned attendances so that we can more efficiently
  prepare practice objectives and member efforts.
* The chassis only lacks a peripherals mounting surface which we plan to print.
  Jeffry and Alec have been trying, without success, to reserve 3D printer time
in the Geisel Library DigitalMediaLab.
* Karina received a T-shirt order invoice of $12/shirt
* Ian says that the Quadcopter team will be using custom scripts to preprocess
  their camera and sensor data before feeding it into their autopilot
controller. He suggests we think about the same approach and maybe avoid ROS
because using it to preprocess data requires a steep learning curve.

## Daily Objectives
Or primary objective is to test that the current chassis, power distribution,
and RC control system is functional by manually driving the vehicle. We should
also use this time to familiarize ourselves in carefully controlling the
vehicle. Our second objective is to setup the second RPI2, especially RTK, so
that it can be used to configure sensor inputs with the Navio+. We also plan to
run basic functionality tests with the sensors. Moreover we plan to solder
together the ultrasonic filter and PWM-PPM converter. We will also continue to
work with Mission Planner to send RPI2 Navio+ outputs to a servo. Finally we
need to discuss logistics about the attendance list, T-shirt sizes, fundraisers,
properly sharing work on gDrive, and 3D printing options.


## Progress Reflection

We were only able to complete 2/6 of our initial daily objectives.

**Peripherals**

* Today Ultrasonic Sensors (model MB7360) were connected using the pins and
  power supply from the battery. Christian, Wilfred, and Jeffry read outputs on
the a digital multimeter for quick prototyping. Results: It appears that the
voltage and distance from obstacles scale linearly (this scaling coefficient
depends on the input voltage according to the schematic). This also appears to
be sensitive to wind, which could be problematic. This fact still needs to be
verified. Measurement equipment may need to be double checked using
oscilloscope. Also, output options need to be discussed with team.
   - Analog Voltage: Simple implementation. May be noisy (can be fixed with
     capacitor low-pass filter). Has compatibility issues since RPI does not
have analog input ports. An ADC can be made to fix this. May have some circuit
building overhead. Good if you want to learn about analog circuit stuff.
   - Pulse Width Modulation: May require change from PPM to PWM. This also may
     be fixed with a differentiator + diode circuit. Connection via PWM and PPM
not verified on either sensor-side or RPI-side.
   - Serial Connection: Serial connection is RS232 Serial protocol. Settings are
     on the schematic sheet for baud rate etc. RPI doesn't take RS232
Connection. RS232 connection is rather old and many computer may not have ports
that support this connection. (Jeffrey's does). A converter from RS232 to I2C or
other compatible communication protocol is necessary.

* Jeffrey soldered header pins to both ultrasonic sensors.

* Wilfred continued to follow Emlid’s RTK setup instructions, installed the RTK,
  but got stuck configuring its first time setup.

**Hardware**

* Jeffry and Alec ran the chassis using the RC control system. The wheels spun
  but output no torque and the vehicle wouldn’t move on the ground. Jeffry
confirmed that the front and rear wheel differentials were too loose so
tightened. Afterwards, more motor power was transferred to the motors and the
chassis works well with plenty of power and speed!

**Software**

* Clark and Alec continue trying to send RPI2 Navio+ outputs to a servo. Since
  Alexander is not at practice, they install APM Planner 2.0 (The Descendant
Software of Mission Planner) then try to SSH from an OSx machine. They install
AngryIP and nmap but cannot work either because Clark's Macbook doesn't have an
ethernet port. Not giving up, Clark attempts to SSH to the RPI2 over LAN WIFI,
but is unfamiliar with Alexander's modifications to the RPI2.

Attendance: Alec, Alex, Chris, Clark, Jeffry, Wilfred

\- Alex Hermstad & Alec Guthrie (February 24, 2016)
