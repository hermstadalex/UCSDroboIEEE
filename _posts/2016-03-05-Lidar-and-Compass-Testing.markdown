---
title: "Practice #24: Lidar and Compass Testing"
date: 2016-03-05
layout: post
categories: jekyll update
---

{% include image.html
            img="http://i.imgur.com/vYfwuQj.jpg"
            title="title for image"
            caption="Example Picture of the PPM Encoder"
            height="449px"
            width="337px"
%}


## Updates

* Reimbursements received for Wilfred and Alec
* T-Shrits order delayed by internal IEEE logistics
* Library 3D printers used to print bottom of case
* New parts: 3DR PPM encoder
* Competition date announced: September 17, 2016

## Daily Objectives

Today’s objectives are to progress through MissionPlanner’s Mandatory Hardware
Configuration, and continue familiarizing ourselves with methods to read Lidar
and Ultrasonic inputs to the RPI2 or MissionPlanner software. Other daily
objectives, if we have extra time, include adding a checklist of steps to finish
the Chassis Maintenance Guide and also working through more of the Udacity AI
course.

## Progress Reflection

**Peripherals**

* During this practice, Alex and Karina worked on the Lidar sensor and
  connecting it to the Navio+. It was decided to use USB powering of the lidar.
It was also decided to use the Serial ports on the lidar as opposed to the I2C,
as the I2C port will have been taken up by the compass sensor. The next steps
are to power Lidar using USB, connect Serial ports to RPI, configure on Mission
Planner, and test input on Mission Planner.

* Alec and Alexander worked on the compass on the compass in the Navio+. The
  internal compass on the Navio+ is giving a Compass Variance error in Mission
Planner which means that in the EKF (Extended Kalman Filter) solution, the
compass heading disagrees with heading estimate from other inertial sensors.
During compass calibration, they found that the axis does not move when they
rotated the device and thus, they were not hitting the calibration points
(example from the Mission Planner website). [Compass
Calibration](http://planner.ardupilot.com/wp-content/uploads/sites/5/2015/12/MissionPlanner_CompassCalibration_LiveCalibrationScreen.png)

*  In addition, our compass heading from the main Mission Planner Flight Data
   screen seems to be drifting and not consistently pointing to north. We have
also tried to plug in an external compass module but have not had much success
connecting to it.

* Compass calibration is critical since the compass provides the primary source
  of heading information. A temporary solution could be to disable the compass
and rely solely on the GPS for heading information but its reliability would
need to be tested.

* Another point of information is that Chris says it might be an addressing
  issue if we are connecting to the internal Magnometer sensor using I2C. Ian
says that it's possibly just MissionPlanner that's messing up if we do get raw
RPI2 readings, but nothing in the mandatory hardware calibration.

Attendance: Alec, Alex, Alexander, Karina

\-Alex Hermstad (March 05, 2016)
