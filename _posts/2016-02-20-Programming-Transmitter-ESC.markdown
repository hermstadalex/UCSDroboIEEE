---
title: "Practice #20: Programming ESC and Transmitter"
date: 2016-02-20
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
- Timeline Gantt updated
- "Power How-To" finished
- Website: Up to practice #18 is live and the first 6 practices have photos
- Alec reestablishes contact with Oren who offers plenty of suggestions:
   * Maxbotix sonars are not useful a speeds necessary to be competitive ~
     15\-20mph. Maybe ... maybe the sensors could help if we calculated the
     vehicle’s travel distance to be within 4 meters during a reading.
   * The Navio+ can’t really extend the APM decision making capabilities. If
     anything MAVROS/MAVLink is probably the simplest option.
     [MAVLink Tutorial](http://dev.ardupilot.com/wp-content/uploads/sites/6/2015/05/MAVLINK_FOR_DUMMIESPart1_v.1.1.pdf)
   *  Another option could be to emulate sensor inputs and input them as an APM
     decision function?
   * For OpenCV we will need a software that goes beyond object detection and
     provides decision making. Without a decent way to implement info received from
     OpenCV to APM most of our efforts will go unnoticed in the final product. Also,
     the APM ties up a lot of computing power and might not offer enough resources
     for OpenCV. Lastly, the [CVRR lab](http://cvrr.ucsd.edu/) is probably a better
     OpenCV resource instead of the Coordinated Robotics Lab.

## Daily Objectives

Today our objectives are to continue progressing our timeline. In order of
importance, first the ESC and battery must be secured to the chassis. Second,
the RC Controller and ESC should be calibrated/reprogrammed. Third, we need to
get servo/ppm outputs that respond to GPS changes. Finally, we need to prepare
the Lidar and Ultrasonic sensors for the Navio+ by making connection schematics
and learning their data transfer protocol.`

## Progress Reflection

We were only able to complete 1/3 of our initial daily objectives.

**Peripherals**

* Wilfred, Christian, and Karina updated the Multifunction LCD Programming Box
  software to version (V105_150408) and can now interface setting via USB on
computer (USB Software Link Successful).

* Alec continued trying to reprogram the RC Transmitter but found that the
  dongle drivers don't work on Windows 10 because the PL-2303HXA dongle (chip
manufacturing code is LFC-14-08-3A for year 14, week 8, 3rd edition) is
discontinued. Driver support [stopped after Windows 7.](http://www.prolific.com.tw/US/ShowProduct.aspx?p_id=225&pcid=41) Alexander
helped Alec and installed the drivers and T6config.exe on a Windows XP virtual
machine. The dongle was successfully recognized and they accessed a live
calibration of the RC Transmitter. However, T6config.exe is archaic and they
couldn’t figure out how to reprogram the Transmitter’s bindings. They’ve made
notes of the receiver's current bindings but don't plan on using the dongle to
reprogram the RC Transmitter.

* Jeffry, Wilfred, and Chris created a PWM-PPM schematic to interface the
  ultrasonic sensor outputs with the Navio+.

**Hardware**

* Jeffry and Sanil mounted the ESC and Motor using velcro. Then Sanil educated
  himself about the vehicle’s power distribution and Jeffry made measurements
for the Peripherals Mount.

**Documentation**
* Karina polled the team’s opinion and chose the most popular image as our logo.

* Alex added the team logo on the landing page, included up to practice #18 on
  the website, added bio pictures for everyone, and added a few photos for the
early practices.

* Alex suggested the team adopt a shared list to keep track of attendance
  (instead of using social media)

Attendance: Alec, Alex, Alexander, Chris, Jeffry, Karina, Sanil, Wilfred

\- Alex Hermstad & Alec Guthrie (February 22, 2016)


\- Alec Guthrie (February 6, 2016)
