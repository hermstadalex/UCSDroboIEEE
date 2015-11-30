---
layout: post
title:  "Practice #6: Platform Decisions"
date:   2015-11-26 23:29:13 -0800
categories: jekyll update
---

The team focused on determining which platform best fit the team's goals and
proves that basic motor control can be accomplished. During practice #6, we
consolidated each member's research for a platform and ultimately agreed upon
the Navio+
  
### Goals

In order of importance:

1. Basic I/o
  - One fundamental goal was to have a vehicle that completed the track
   regardless of method or speed.
2. GPS
3. Machine Vision
  
#### Third Choice:
Inforce6410
  
#### Second Choice:
Erle-Brain 2
  
#### Honorable Mention:
Another option for a control platform would be the SnickeDoodle, due to its
being small, powerful, compatible, and started by a community of makers. It
features 179 I/O ports. Unfortunately it was still being funded via crowdsource.
  
My remaining top two suggestions were the Erle-Brain2 and BeagleBoneBlack. The
EB2 was literally made to conquer the niche exposed by BBB auto-pilot platforms,
so it meets basic I/o, easily integrates GPS+APM, and packs plenty of power for
image processing. The only downside is that it's community is new, specific
support was difficult to find, and there are bound to be bugs. Plus, it's
tailored header pins and connections could be a problem if used without
specifically compatible hardware (like last year's experience with the Pixhawk).
  
The BBB is an on-board computer meant for embedded applications. It's got plenty
of I/O pins, full camera+openCV support, and much more expandable than the EB2
through the use of capes. Unfortunately, most of its community migrated to the
EB2, and the suggested GPS module must be hand soldered.
  
#### Final Decision: Navio+
The team collective agree upon the Navio+ because it is more extensible and is a
better learning environment than Erle-Brain2 and Inforce6410. This would also
mean that our skills gained from using the Raspberry Pi with Navio+ could be
applied to hobbies outside of Robomagellan. In case of trouble
shooting, there is vast online resources and documentation for many years. 
  
\- Karina Nino
