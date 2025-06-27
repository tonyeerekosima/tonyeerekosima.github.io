---
layout: post
title: Recovery Shop Writeup - BCACTF 2025
description: My writeup for the Foren/recovery-shop challenge in BCACTF 2025
image: "/assets/img/recovery.png"


categories:
- Writeups
- BCACTF 2025

tags:
- foren

date: 2025-6-23 00:00 -0500
---

# Intro
Greetings! In this writeup, I’ll walk through my approach and solution to the Recovery Shop challenge from BCACTF 2025.

Category: Foren

Difficulty: Easy   

# Challenge
Once opened, the challenge presents us with the following: 

![This image would be a screenshot of the challenge info](/assets/img/shop.png). 

The challenge provides a file containing data and information that I couldn't read because it was a HEIC file and my Windows didn't have the extension. I wasn't about to download it
because that would've wasted precious time. So, I used some forensics thinking instead. 

# Approach
Typically, the first step I would take to solve a CTF would be examining the file and determining what type of challenge it is and techniques to solve it. But since the file is virtually meaningless,
now I just needed to use my brain. I knew that .heic is not a common file type by any means, so I figured converting file types might show me the challenge to solving it.

PNG, JPG, JPEG, and PDF are all common ones I could've attempted. But I was googling "heic to" and it autocompleted it to JPG, so I decided to try that one first. 
After finding a converter that didn't make me remove my adblocker, I got this screen: 

![This image would be a screenshot of the challenge info](/assets/img/convert.png). 

When downloading the provided images, it's shown as a zip file, which everyone knows how to deal with. Extract All and examine all the files.

![This image would be a screenshot of the zip files' contents](/assets/img/zip.png) 

When I went through it, I was able to find out all the info I needed. The first 5 files were dummy files, but the very last one as a very hierarchical-staircase display of
the flag.

![This image would be a screenshot of the zip files' contents](/assets/img/OCR.png) 

# Solution
The flag is bcactf{th!ss_@!e_83klts_fr_b!n@na_f$_l@gOrz}, as shown in the image. This challenge was an assessment of forensic knowledge and computing instincts. This was a good challenge
and I really enjoyed it. 
