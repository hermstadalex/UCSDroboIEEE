---
title: "Practice #16: Research Power Distribution and Sensor Integration Through
Navio+"
date: 2016-02-06
layout: post
categories: jekyll update
---

Updates
-------

-   More parts arrived: the second, undamaged, shipment of pinion gears as well
    as the two Maxbotix Ultrasonic sensors.

-   The Rpi2/Navio+ case is ready to be printed. We just need to submit early
    reservations for the library 3D printers and use Jeffry’s schematic.

-   Alec confirmed with the IEEE project head Ian, that Karina’s team designs
    can use the IEEE logo so long as the logo itself is not modified.

 

Daily Objectives
----------------

Despite the importance of completing the timeline, the discarding of last
practice’s progress was disruptive. Nonetheless, we followed the timeline
established last practice, so today’s objectives were to research power
distribution for the vehicle and research how the Rpi reads sensor inputs
from the Navio+ GPIO Pins. By accumulating knowledge and preparing how-to’s
we can make the most of practice once the battery and motor are shipped.

 

Progress Reflection
-------------------

SST

-   In order for the Rpi2 to interact locally with the Navio+ and read inputs
    from the Navio+ pins the Ardupilot Rover firmware must be installed. This is
    different from using a ground control station software like Mission Planner
    to interact with the sensors on the autopilot controller.

PST

-   Found that the ultrasonic sensor uses PWM and can connect the the GPIO pins
    of the Navio+.

HST

-   Created a google document to accumulate researched [power distribution
    knowledge](<https://docs.google.com/document/d/1fFmpxXabo6tUiT5DuqbfEh6qTOSzbjdLNjXhHZG77Ro/edit>).
    The document has a fast-stats table at the beginning and the remainder is a
    step-by-step guide.

-   Improvised their first power distribution schematic:
    
![alt
text](http://i.imgur.com/U5qHzwW.jpg
"Logo Title Text 1")


-   Watched [an informational RC power
    video](<A%20good%20summary%20of%20necessary%20components%20in%20RC%20power%20distribution:%20https://www.youtube.com/watch?v=DraFgiDELjI>)
    and learned that the Navio+ power module acts as a BEC for the Navio+/Rpi2
    but otherwise we will likely need a BEC for the steering servo.

 

### Attendance

Alec, Alex, Clark, Jeffry, Sanil

 

\- Alec Guthrie (February 6, 2016)
