---
layout: post
title:  "Making A Static Website"
date:   2017-10-13 13:56:09 -0600
image: https://i.imgur.com/J3ik2HF.png
---



It is finally time to make my website. I decided to host my website on GitHub pages and apply a Jekyll theme to it.

Goals

1. Host my site using GitHub Pages
2. Apply a theme
3. Upload site to Github Pages
4. Update my site using Atom/Terminal `git clone` `git add` `git push` and `git commit`

## 1. Making a Github page

GitHub offers every user one free hosted page which awesome because it is free and easy to update. The first thing I did was create a new repository on Github. The repository must be "yourname.github.io". I chose to not initialize it with a readme because I am going to use the README from the theme I download.

## 2. Getting a theme

I searched Jekyll themes on Google and found [Forty](http://jekyllthemes.org/themes/Forty/).


<img src="https://i.imgur.com/Y4MJawu.jpg" alt="Forty Theme" width="500">

Why I chose this theme:

- I love dark themed backgrounds with light text. Nice and easy on the eyes.
- Simple nav bar (one button)
- Posts are prominently displayed and easy to see.

I downloaded the theme, replaced a few things with my own and ran `jekyll serve`.


<img src="https://i.imgur.com/lKoEtkZ.png" alt="Forty Theme" width="500">

Success. I edited the config file to include my information and added my posts to the `_posts` folder. Now I am ready to make my site live.

## 3. Uploading to Github

I hopped on terminal and navigated to the working directory of my project.

I initialized my local directory as a Git repository using `git init`

Then added all of my files using `git add .`

<img src="https://i.imgur.com/JGxo76A.png" alt="TerminalSS" width="500">

I committed the changes `git commit -m "hope this works"`.

Then I went back to github and copied the remote repository's URL, and added it to the origin.

<img src="https://i.imgur.com/FIJDFRJ.png" alt="TerminalSS" width="500">

Bam. I was feeling good. I excitedly ran over to Chrome and typed in the URL for my site, [criticalmatt.github.io](https://criticalmatt.github.io/) and saw this:

<img src="https://i.imgur.com/GyKQO3t.png" alt="bad website" width="500">

Houston, we have a problem. It appears that my HTML uploaded correctly, but not my style sheets. I spent hours troubleshooting this with no success. After consulting with a classmate and my professor I realized that the links to my stylesheets in my config file were inaccurate. I changed them to my github URL


<img src="https://i.imgur.com/GyKQO3t.png" alt="bad website" width="500">

This solved the problem. I ran `jekyll build` again and ran into the same, unstyled webpage.

<img src="https://i.imgur.com/GyKQO3t.png" alt="bad website" width="500">

This stumped me. My professor advised me to try deleting the repo and that solved the problem.

## Success!

<img src="https://i.imgur.com/QOMALA4.jpg" alt="bad website" width="500">

**What I learned**

- How to use Jekyll and apply a theme
- How to host a website using GitHub pages 
