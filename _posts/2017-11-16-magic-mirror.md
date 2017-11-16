---
layout: post
title: Enchanted Objects 
description: Making A Smart Mirror
image: https://i.imgur.com/2HTpMPq.jpg?1
---

# Summary

We made a static website that we ran an old 50 inch TV using a Raspberry Pi 3. The website was all black showed showed only white text/images of:
- the current time, 5-day weather forecast (using OpenWeather API data)
- Current News Headlines from Yahoo! News Denver RSS feed
- upcoming birthdays of students in our graduate program
- a cycle of interesting facts and quotes we found on Reddit

We mounted the TV on a frame made out of Poplar wood we got from Home Depot and placed a 2 way mirror in front of the TV so that only white text from the website showed through.

## Inspiration

Our classroom is very bare as we are the first iteration of students to occupy our new space in downtown Boulder, Colorado. When we started we essentially studied in a concrete box, with whiteboards and tables, and sticky notes on the walls. We wanted to make something using the skills we were learning in our Critical Making class to create ~~something~~, anything, that would make the space a little more interesting. At the time we had just began learning about Arduinos and Raspberry Pi's, small circuit boards that can be programmed and attached to anything to gather and send data. Ty had the idea of creating a mirror that could tell us useful things about the outside world. We also just thought it would be a cool way for us to learn more about code and making stuff.

<img src="https://lh5.googleusercontent.com/FzEuycNiL1u91uGHvHhfcgP8XegMeoOeYnEQEyPiYLlF2JsYHrGGDytuGZ48kI6NGdioCz6dxc5MHz0TU0spg8qzsxSrqnvt0QWVdnQLU-FOuBwzqbtX6uArSEpRNIjgzlVRaFPj" alt="Mirror plan" width="500">


We began by brainstorming ideas of information that the mirror could display. In the spirit of design thinking we thought about the feeling we wanted the mirror to evoke from our audience, mainly stressed out graduate students.

*Side Note:* Before the 15th century, Humans had no means to see what they looked like besides reflections from still bodies of water. The development of high-quality silvered glass allowed for royalty and other rich classes to view their appearance as others saw them, this brought about a monumental change to the human psyche, and civilization as we know it.

In his [book,](http://pegasusbooks.com/books/millennium-9781681772431-hardcover) author Ian Mortimer writes that before this invention, the concept of individual identity didn't exist.  Now we see ourselves everywhere. Through pictures, selfies, and social media, we are constantly analyzing what we look like. The goal of this mirror was to make people think of other things while looking at themselves, instead of over analyzing our appearance like we do so much nowadays. *End Side Note*

## Supplies/Parts

1. Raspberry Pi 3
2. 50 inch TV
3. 50 inch custom cut 2 way mirror glass
3. Frame to hold in the mirror and TV

For the frame:

- 15’ of 1”x3” poplar
- 15’ of 1” x 4” poplar
- a box of pocket screws
- a box of 4" frame screws
- wood glue
- jig
- drill bits
- sand paper

--------- Total Cost: $137



We found some [code](https://github.com/MichMich/MagicMirror/releases/tag/v.2.1.3) on GitHub to help us through this project. We downloaded that code, updated the API information for weather, added in Google Maps data about our location, added the birthdays of our classmates, plugged in our favorite mind-blowing facts and inspiring quotes. For example, did you know that we are closer in time to T-Rex than a T-Rex is to a Stegosaurus?

## Photos

<img src="https://lh5.googleusercontent.com/FzEuycNiL1u91uGHvHhfcgP8XegMeoOeYnEQEyPiYLlF2JsYHrGGDytuGZ48kI6NGdioCz6dxc5MHz0TU0spg8qzsxSrqnvt0QWVdnQLU-FOuBwzqbtX6uArSEpRNIjgzlVRaFPj" alt="Mirror plan" width="500">

Our initial sketch. As this project progresses we want to implement other features, such as the Google Maps API for bus times, and connecting the mirror to a slack channel so that other students can post things that will appear on the mirror.

<img src="https://i.imgur.com/D0dOrT5.jpg" alt="Website Up" width="500">

Getting the website running using the [code](https://github.com/MichMich/MagicMirror/releases/tag/v.2.1.3) we found on GitHub.

<img src="https://i.imgur.com/WUL2Yrs.jpg" alt="Website Up" width="500">

We took the back off the TV to make sure we had enough room to place the frame around it.

<img src="https://i.imgur.com/TliiZFj.jpg" alt="Website Up" width="500">

We used the back of the TV to test   the dimensions of the frame.

<img src="https://i.imgur.com/UkC6a9y.jpg" alt="Website Up" width="500">

While trying to remove the bezel of the TV so allow for less light to escape, we cracked the screen.

<img src="https://i.imgur.com/546Sj1C.jpg" alt="Website Up" width="500">

Pocket holes for the front facing corner of the frame.

<img src="https://i.imgur.com/zmVXfSp.jpg" alt="Website Up" width="500">

Clamps secured the frame to the table while we screwed and glued the back of the frame to the front.


<img src="https://i.imgur.com/3Roxgjo.jpg" alt="Website Up" width="500">

The back of the frame.

<img src="https://i.imgur.com/chRtWYe.jpg" alt="Website Up" width="500">

The 2 way glass laid down in the frame.


<img src="https://i.imgur.com/QfwrO3r.jpg" alt="Website Up" width="500">

Version 1 of the mirror went on display at an event held during homecoming.

<img src="https://i.imgur.com/2HTpMPq.jpg" alt="Website Up" width="500">

The brightness was a bit low because we had to switch to a smaller TV last minute after our 50 inch screen cracked.


### TO BE CONTINUED...
