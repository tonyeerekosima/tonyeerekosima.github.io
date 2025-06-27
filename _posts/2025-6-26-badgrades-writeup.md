---
layout: post
title: Bad Grades Writeup - BCACTF 2025
description: My writeup for the Misc/bad-grades challenge in BCACTF 2025
image: "/assets/img/transcript.png"


categories:
- Writeups
- BCACTF 2025

tags:
- misc

date: 2025-6-26 00:00 -0500
---

# Intro
Greetings! In this writeup, I’ll walk through my approach and solution to the Bad Grades challenge from BCACTF 2025.

Category: Misc

Difficulty: Easy   

# Challenge
Once opened, the challenge presents us with the following: 
![This image would be a screenshot of the challenge](/assets/img/writeup.png)

The challenge provides a file containing a list of grades, percentages, and classes that the student (Josh) has taken, titled transcript.txt 
![This image would be a screenshot of the challenge file](/assets/img/transcript.png). 

The challenge provided no hints, so this one is purely based on CTF instincts and experience. When opening the transcript.txt file, everything appears normal, but there's
always some trick with a CTF.

# Approach
My first instinct was the numbers and letters, leading me to believe that there was some cryptography trick to this. So I tried to conenct the letters and numbers together and use a cipher decoder
to decipher it. When aligning all the letters and grades in chronological order, you get: 73c31f65d33f70c73c49f23f43f31f28f61d53f24f, which is hexadecimal. But, when I translated it, I got this:

![This image would be a screenshot of the decoded hex values](/assets/img/decode.png), which is: sÃeÓ?pÇ<Iò?Có(öSòO 

That outputs pure garbage, so that's a major clue that's not the method. But the given info definitely gave off the vibes of a crypto CTF, so I switched methods.
I tried just focusing on the numbers. I then realized that the numbers were in the 0-99 range, so all of them could be the hex itself. I decided to list all of
them in order from top to bottom, and try to decode them. And there it was!

![This image would be a screenshot of the decoded numbers](/assets/img/flag.png) 

## Solution
The flag is `bcactf{s1e3psI#C1(aS$}. This challenge was an exploration of cryptographic knowledge and basic decoding methodology.` I really liked it and it was fun to do.





