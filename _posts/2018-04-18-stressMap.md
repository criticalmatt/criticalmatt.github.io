---
layout: post
title: Stress Map
description: Visualizing feelings with node and a Raspberry Pi
image:  https://i.imgur.com/2nqNsAi.gif
---

## What

We made an application that displays the current stress level of our masters program. There are two buttons, stressed, and not stressed. Red dots represent stressed people, blue dots represent represent relaxed people.

<iframe src="https://player.vimeo.com/video/265508682" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
<p><a href="https://vimeo.com/265508682">stressMap</a> from <a href="https://vimeo.com/wasgunnabut324">Jim Murphy</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

## Why

Grad school is stressful. Design sprints, group projects, and personal projects are constantly overlapping. Hearing "I have so much work to do" is as common as someone walking in with iced coffee. We created a way for people to express stress and visualize the collective stress levels of our program. The goal of is to take a negative thing like stress, and create a relaxing visual that is easy on the eyes. And, slamming an analog button feels great sometimes.

## How

We set up the two buttons on our Arduino, and then connected it to a Raspberry Pi that ran a webpage for our sketch, received data from the Arduino, and communicated to and from our node server via web sockets.

This project allowed me to learn a variety of new javascript libraries and frameworks, including:

- [node.js](https://nodejs.org/en/) to create a server on our pi
- [express.js](https://expressjs.com) to create the framework for our node app
- [pug](https://pugjs.org/api/getting-started.html) (formerly Jade) to make a template for our site
  - [pug translator](https://html2pug.herokuapp.com/)
- [socket.io](https://socket.io/) to emit signals from the browser to our server
- [johnny-five](http://johnny-five.io/) to relay information from the Arduino to Raspberry pI
- [p5js](https://p5js.org/) to create the visualization using data from our buttons and web sockets.
