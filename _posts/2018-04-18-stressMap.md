---
layout: post
title: Stress Map
description: Visualizing feelings with node and a Raspberry Pi
image:  https://i.imgur.com/2nqNsAi.gif
---

## What

We made an application that displays the current stress level of our masters program. There are two buttons, stressed, and not stressed. Red dots represent stressed people, blue dots represent represent relaxed people.

![stressMap Pic](https://i.imgur.com/qNq53gf.jpg?1)

<iframe src="https://player.vimeo.com/video/265508682" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
<p><a href="https://vimeo.com/265508682">stressMap</a> from <a href="https://vimeo.com/wasgunnabut324">Jim Murphy</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

## Why

Grad school is stressful. Design sprints, group projects, and personal projects are constantly overlapping. Hearing "I have so much work to do" is as common as someone walking in with iced coffee. We created a way for people to express stress and visualize the collective stress levels of our program. The goal of is to take a negative thing like stress, and create a relaxing visual that is easy on the eyes. And, slamming an analog button feels great sometimes.

## How

We set up the two buttons on our Arduino, and then connected it to a Raspberry Pi that ran a webpage for our sketch, received data from the Arduino, and communicated to and from our node server via web sockets.

**What is an Arduino?**

An Arduino is a small circuit board with a series of inputs and outputs. They can take in data from the physical world through sensors, and output data to a computer, or to analog things like lights and speakers.

For this project wired two buttons to the Arduino with a breadboard.

![Imgur](https://i.imgur.com/uoktyfx.png?1)

**What is a Raspberry Pi?**

A Raspberry Pi is a small computer that can be plugged in to a TV or monitor. It can be used for anything a normal computer does, but in our case we used to run an application that took in data from our Arduino and displayed a webpage with a visualization of stress.

**What is a Node App?**

A node application is a server side program that allows for the creation of real time web applications. In other words, it creates dynamic, non static sites.

![Node Visualization](https://i.imgur.com/fmMyJiy.png)

Unlike static web sites, node can handle multiple requests at once and handles requests asynchronously.

This project allowed me to learn a variety of new javascript libraries and frameworks, including:

- [node.js](https://nodejs.org/en/) Is a javascript framework that can transform your local computer into a server. We used this to create a server, tested it on our local computer, and then uploaded it onto our pi.
- [express.js](https://expressjs.com) to create the framework for our node app. Express makes it easy to handle requests to and from the server, and allows us to create "routes" to different pages.
- [pug](https://pugjs.org/api/getting-started.html) (formerly Jade) to make a template for our site. Essentially pug is a language that allows you to set up the skeleton format of a page, and express is used to to update the content dynamically using keys and values.
  - [pug translator](https://html2pug.herokuapp.com/) Pug is just another way of writing HTML, so it is handy to use a converter to check our syntax.
- [socket.io](https://socket.io/) to emit signals from the browser to our server. Sockets are what allows websites to be updated from two different browsers at once. The most common usage of sockets is instant messaging applications.
- [johnny-five](http://johnny-five.io/) to relay information from the Arduino to Raspberry Pi.
- [p5js](https://p5js.org/) to create the visualization using data from our buttons and web sockets. P5 is a javascript library that allows creative coding for javascript. The closest thing it can be compared to to is Java, which is used in Processing. P5js is really useful for creating visual representations of data for web applications.

This is how everything fits together.

![Imgur](https://i.imgur.com/FoeDVd1.jpg?1)

The code for the project can be found [here on GitHub](https://github.com/wasgunnabut/stressMap).

I worked on the code with my friend [Jim Murphy](jimmurphy.studio).

The stressMap is currently up and running 24/7 on one of the projectors in our classroom. I will update this post in a couple weeks to see how it was received by program. Should be an interesting add on to finals week.

![StressMap Porjector](https://i.imgur.com/XmWO5ow.jpg)
