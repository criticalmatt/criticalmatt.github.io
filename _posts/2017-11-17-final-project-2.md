---
layout: post
title: Smart Nozzle
description: Final Project Plan Pt. 2
image:  https://i.imgur.com/mLNNUfT.jpg
---

# Summary

For my final project I will create a Smart Nozzle that will help my mom water her plants more efficiently. It can potentially also have educational value in that it will allow her to see how much water she is using for each plant. I hope that this will

- decrease the amount of overwatering
- decrease water waste
- decrease the amount of time my mom spends watering each plant
- increase plant health
- increase knowledge about the watering needs of plants

**Features**

- A nozzle with three inputs (buttons)
- A solenoid valve to control the flow of water.
- A meter that shows how many gallons are passing through the nozzle
- Three LED lights green/amber/red that notify's the user when the plant is done being watered.
  - Preset values for drought and non-drought plants displayed in gallons.
  - Preset values for newly planted vs mature plants.


**Materials**

- A nozzle
- Arduino Uno
- Solenoid valve
- 3 LED lights green/red/amber
- Water Meter (gallons)
- Relay


**Research**

- Average amount of water needed weekly for drought / non drought plants

**Sketch**

![nozzle sketch](https://i.imgur.com/IA93pwL.jpg?1)

## What I've done so far

To gain a better understanding about soil moisture levels and Arduino's, I made a [self watering plant](criticalmatt.github.io/2017-10-15-its-electric.md). This helped me understand how to connect an Arduino to a sensor, and how important it is to have the right amount of water in the soil of a plant.

I spent some time at Boulder Nurseries talking to employees about watering. The three main factors that affect watering are:

- soil type/density
- exposure to light
- maturity of plant

I found that the nurseries I visited had created their own scale on which they used to let customers know how much water each plant needed.

![water tag](https://i.imgur.com/2uJIRm1.jpg?1)

![water tag 2](https://i.imgur.com/mRf2d2o.jpg)

There were labels like medium to moist, or light.

My idea was to assemble a database of these factors. Then create a system of sliders with inputs such as

- size of plant
- amount of light exposed to
- soil type

The goal would be to make an algorithm that gives you the exact amount of water needed for each of your individual plants, and then program that value into the nozzle, allowing users to walk up to any plant in their garden, press a button, and have the nozzle deliver the perfect amount of water to your plant.

![sketch](https://i.imgur.com/T4kZMBO.jpg?1)

However, this will be a project that needs to tackled next semester. For now, I am going to focus on making a prototype that has 3 different preset values based on gallons of water used for drought resistant and non drought resistant plants, use the solenoid valve to control the flow of water, and connect LEDs as output devices.
