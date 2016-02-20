---
title: "Practice #18: Soldering and Powering the Servo"
date: 2016-02-13
layout: post
categories: jekyll update
---

Attendance: Alec, Alex, Alexander, Karina, Wilfred

## Updates

- New Orders: The properly fitting pinion gear was not ordered. We found one
  that came in the same package as the motor.

- New Parts: Both BECs arrived

- Building: Alec glued the tires to the wheels

## Daily Objectives

Continue to work towards timeline goals. Specifically our goals were to continue
establishing power distribution even though the chassis wasn’t expected to be
built, to receive GPS data through the RPI2 instead of the Mission Planner
software, and to make schematics connecting the ultrasonic sensor to the
Navio+/RPI2. For power distribution our objective was to solder connectors onto
the BEC’s and solder the ESC to the motor. Then to power the radio received and
prove that servo can be controlled by radio remote. As well as power the Navio+
servo rail and prove that the servo’s can be controlled by the Navio+.

## Progress Reflection

**Software:**

* Did research on APM Rover and how it would fit together with developing the
  system.

**Perpherals:**

* Downloaded the Navio drivers and example codes by running the following
  command: git clone https://github.com/emlid/Navio
* Ran the [GPS example
  code](https://trello-attachments.s3.amazonaws.com/56bfad65a530f4ede230f87a/828x520/4de8444f2ab4f1ecf9a6d0d12d4a80cc/pi_gps_ssh.jpg)
through SSH and received GPS data from the Raspberry Pi. 
* Connected the BEC to the servo power rail on the Navio+ and attached a servo
  to channel 5. Using Mission Planner (in the servo tab), we were able to turn
the motor on and off and switch directions. The values next to the toggle the
output signal voltage which can reach 5V depending on the parameters.
* Learned that the 5V dc rail can be used to power the lidar and ultrasonic
  sensors. They will need filters: the ultrasonic sensor’s filter will consist
of a 10ohm resistor between the DC source and the DC input, and a 100uF
capacitor between input and ground. The lidar sensor will consist of a 1000uF
capacitor (recommended by an IEEE member that is in Grand PRIEEE) between the DC
input and ground.
* Trying to make receiver work, but no power to receiver. Tried to power from
  controller but it wasn’t enough power. Voltmeter difference when testing pins,
but was very insignificant (0.2 V). Schematics for hooking up sensors to
computer.

![alt
text](https://lh5.googleusercontent.com/CZw4KGPk4Lbsq-7Ae8jfbBsqb4bazCHNGJSB7X5yhBO7iFqsDnYZmu8Mjo69iS8dsoYFfg=w1816-h851
"Logo Title Text 1")



**Hardware:**

* Alec and Karina both learned to solder today. We began soldering old resistors
  together, then tested our dexterity by soldering components on adjacent IC
header pins, and finally added old ICs to a PCB soldering board. Meanwhile we
learned about the importance of tinning and that flux determines how easily
solder flows.
* [Proper
  Temp](http://electronics.stackexchange.com/questions/1980/what-s-the-proper-soldering-iron-temperature-for-standard-031-60-40-solder)
* [Soldering
  Guide](http://store.curiousinventor.com/guides/how_to_solder/cleantip)
* Now practiced, Karina and Alec soldered on male XT-60 connectors to the BECs
  and Alec finished Karina's work soldering the ESC to the motor.
* The pinion gears do not need to be reordered. They don't fit, but there were
  gears included in with the motor package all along! 

\- Alec Guthrie (February 6, 2016)
