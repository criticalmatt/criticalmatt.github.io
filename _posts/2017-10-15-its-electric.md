---
layout: post
title: It's Electric!
landing-title: 'Autonomous Plant'
nav-menu: true
description: Self Watering Plant 
image: https://i.imgur.com/jCDUD51.jpg
author: null
---



For my first Arduino project I wanted to advance my final project by creating an autonomous plant that knows when the soil is dry, and delivers water to it until it is at the optimal moisture level.

**Sketch**

<img src="https://i.imgur.com/pT3fDDN.jpg|width=100" alt="sketch" width="400">

**Goals**

- Use a soil moisture meter to test the soil and get readings.
  - Determine the optimal soil moisture level as well as the
- Relay those readings to an Arduino
- Create a watering system that will deliver water when the plant needs it.

## Inspiration

A few weeks ago I bought three plants from Home Depot.


<img src="https://i.imgur.com/NR6OIQb.jpg" alt="myplants" width="500">

It was some well needed foliage in my otherwise lifeless apartment. According to the lady in the garden section, these plants should get about 1 cup of water a week. I watered all of them the same amount everyday. After 9 days, one of my plants began losing a lot of leaves. Then this happened.


<img src="https://i.imgur.com/wCpagy2.jpg" alt="Dead plant" width="500">

Man down. After only one week I had managed to kill 33% of the plants in my house. The leaves began falling out after about 5 days and were completely gone after 7. I gave my mom the diagnosis and she confirmed that I had over watered the plant. I was surprised how fast I failed at being a plant owner. This was the inspiration for my project. I clearly am not fit to be a plant parent, so I decided to pass the responsibilities to an Arduino. I browsed [Instructables](http://www.instructables.com/) and YouTube for inspiration and found many people who had already created an arduino watering system. The issue was that all of the examples I found required a 3-6v submersible motor.



<img src="https://image.prntscr.com/image/4iDcuybuRCezVOKiBGMUgA.png" alt="Motor" width="400">

I shopped around the internet, and the fastest I could have one delivered was 3 weeks. Way too long. Using a motor was not an option, so I pivoted. I found another [tutorial](http://www.instructables.com/id/No-Pump-Automatic-Watering/) that didn't require a pump, and decided to base my project off this one. Essentially, it is a gravity powered watering system that takes water from a hanging reservoir and delivers water through a small tube. I placed a Sparkfun order, made a trip to the local nursery, and got started.

-------

**Supplies**


- Spider plant. I chose this plant because NASA studies have shown that spider plants are among the best for filtering harmful toxins and pollutants from the air.
- Arduino Uno
-  5v USB plug for power
- ~~3-6v Water pump and hose~~ Servo motor
- Soil moisture sensor
- Transistor / Low ohm resistor
- A water bottle
- Hot glue gun
- Zipties

While I was at the nursery I asked an employee how I can monitor the soil moisture to know when the spider plant I bought has enough water. She sold me an analog soil moisture sensor with the plant for 50% off after I described my project to her. Score.



<img src="https://i.imgur.com/SAPAtUE.jpg" alt="sensor" width="450">


This allowed me to then interpret the readings from the serial monitor to know when the soil has a sufficient amount of water.



**Configuring the soil moisture sensor**

I ordered a soil moisture sensor from Japan from Amazon. When I got it, the first thing I needed to do was determine the sensor values for when the soil is appropriately wet, and too dry (needs water).


I found an [instructable](http://www.instructables.com/id/Soil-Moisture-Sensor/) that showed me how to set up the sensor to get readings from the soil. I set it up and it looked like this.


<img src="https://i.imgur.com/jCDUD51.jpg" alt="sensor" width="450">


Over a few days I used both sensors and recorded the readings from the serial monitor to determine that the sensor values for wet soil and dry soil.

**Sensor values**
- dry value: 695
- wet value: 395

**What I learned**

- how to connect a soil moisture sensor to an Arduino
- how to read the different values and interpret them based off the analog soil meter

-------

**Creating the watering system**

I used a smart water bottle as a tank because I ~~decided that my plant deserves the highest quality electrolyte/mineral water~~ found an empty one in the recycling bin.

I cut off the bottom and poked two holes on each side. I then tied a string through the holes to make a a handle that would hang on a hook.

I used a box cutter to poke a hole in the cap of the water bottle and then superglued a 10inch long plastic hose to the cap. Water reservoir ready.

I hung the water bottle upside down to the window sill in the corner of my studio. Then I superglued the servo motor to the wall, ziptied the hose to the motor and angled it over the pot.

**Connecting the Electronics**

I continued to follow the [instructions](http://www.instructables.com/id/Soil-Moisture-Sensor/)
and set up the electronics as follows.

- Analog Input 0 - Sensor Pin
- Digital I/O 2 - Sensor +
  - This output pin is configured to power the sensor so that the moisture sensor can be powered directly from the Arduino.
- GND - Sensor GND
- Digital I/O 3 - Servo Wire
- 5V - positive Servo Wire
- GND - negative servor Wire

I uploaded the code he provided and began tinkering with it in Arduino. Here I ran into problems. For some reason the sensor was only reading values between 900 and 1000.

I asked my professor for help and we determined that for whatever the reason, my soil moisture sensor was not working correctly.

*Lesson: Cheap electronics from Japan break easily*

So, I ordered a new soil moisture sensor from Sparkfun.



----

## Conclusion

*To be continued when I configure the new soil moisture sensor*
