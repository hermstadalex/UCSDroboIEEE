---
layout: post
title:  "Practice #5: Platform Decisions"
date:   2015-11-16
categories: jekyll update
---

[This Week's
Powerpoint](https://docs.google.com/presentation/d/1lXwgx6CmjfgPG5dmoYTXs09DMjWjsoz3uhJZBkoQ8WQ/edit)

The team focused on determining which platform best fit the team's goals and
proves that basic motor control can be accomplished. During practice #6, we
consolidated each member's research for a platform and ultimately agreed upon
the Navio+ Raspberry Pi. In addition to the choice of this platform, sub-teams
were also assigned in according to a Software, Peripherals, Hardware, as well as
Documentation tasks to help complete the project in a more efficient manner.
  
### Goals

In order of importance:

1. Basic I/o
  * One fundamental goal was to have a vehicle that completed the track
   regardless of method or speed.
2. GPS
  * Once we accomplish basic mobility, our platform should utilize sensors and
  software to maneuver around the obstacles.
3. Machine Vision
  * Machine vision could be implemented after GPS. This would both help
  navigate obstacles, and do the challenges such as the hoop and ramp.

Here is a table with links to the proof of application for each platform in
terms of the above goals:
[Table](https://docs.google.com/document/d/1b8Je1e7etTIbmG10YwVUiDANtwDea94KqdYbaGUoQ6s/edit)
  
#### *Third Choice*:
The **Inforce6410** was notable for being powerful as far as processing power
and speed. It also has literature on ROS implementation. It lacked documentation
and initially it was not made for robotic vehicles. These factors made this
controller an unsuitable fit for our team and project. 
  
#### *Second Choice*:
The **Erle-Brain 2** was created to conquer the niche exposed by Beagle Bone
Black auto-pilot platforms, ensuring that it meets basic I/O, easily integrates
GPS+APM, and packs plenty of power for image processing. The downside to the EB2
is that the community is new. So if any bugs arise support would be difficult to
find. Plus, its tailored header pins and connections could be a problem if used
without specifically compatible hardware.
  
#### *Honorable Mention*:
Another option for a control platform would be the **SnickerDoodle**, due to its 
being small, powerful, compatible, and started by a community of makers. It 
features 179 I/O ports, 2.4 and 5GHz WiFi, Bluetooth, 1GB of RAM, and an ARM
Cortex A9. Unfortunately it was still in production at the time of our decision.
 
#### *Final Decision: Navio+ Raspberry Pi*

![alt
text](http://i.imgur.com/p1A1jy0.png
"Logo Title Text 1")


The team collectively agree upon the Navio+ because it is more extensible and is a
better learning environment than Erle-Brain2 and Inforce6410. This would also
mean that our skills gained from using the Raspberry Pi with Navio+ could be
applied to hobbies outside of Robomagellan. Additionally, as bugs arise,there is
an extensive and well-documented community to help solve these issues. This will allow us to get a basic
robot established early on in the process, allowing us to attempt more daring
technological endeavors in the future of our project.
  
\- Karina Nino
