---
layout: post
title: Glory of the Garden Writeup - PicoCTF 2019
description: A training CTF writeup.
image: "assets/garden.jpg"

category:
- Writeups
tags:
- foren

date: 2025-5-2 00:00 -0500
---

# Intro
Hello everyone! In this writeup, I will be discussing the Glory of the Garden challenge in picoCTF. I will be walking through my thought process and how I found
the correct solution.

# Challenge 
Upon opening the challenge, we are presented with: 

![This image would be a screenshot of the challenge content.](/assets/img/pico.png)

The description is very straightforward, so we know that there is some type of forensic trick hiding within the challenge. The file showed this nice image of a garden, but in CTFs, there's more than meets the eye.
I tried to solve this without looking at the hint.

# Approach
My first thought was to try and extract metadata from it. So, I found an exiftool to do that. I uploaded my file and looked at the metadata, which showed:

![This image would be a screenshot of the file's metadata content.](/assets/img/exiftool.png)

This didn't display anything that looked suspicious or relevant, so my next thought was to try changing the file type. It was originally a JPG, so I tried to switch it to PNG
to see if I would get any hidden hints or tools. And if that didn't work, I would look at the hint. The PNG showed this:

![This image would be a screenshot of the converted file.](/assets/garden.png)

So, that was the exact same as the JPG version, so it couldn't be a file conversion. 

At this point, I decided to look at the hint, and it read "What is a hex editor?". For those who don't know, a hex editor is a computer program that allows a user to examine and read
all the raw binary data within a file. After seeing that, I found a hex editor online that didn't look complicated, and I uploaded the file. This is what it displayed:

![This image would be a screenshot of the challenge content.](/assets/img/hex.png)

This looked promising, so I decided to narrow it down. PicoCTF flags are formatted like picoCTF{flag}, so I searched pico and there it was!

![This image would be a screenshot of the converted file.](/assets/img/hexflag.png)

# Solution 
The flag is picoCTF{more_than_m33ts_the_3y3BdBd2cc}. This challenge taught me about the basics of hex editor usage, and it was fun to do.
