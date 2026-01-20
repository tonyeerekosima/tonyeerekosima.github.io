---
layout: post
title: Beginner CTF Toolkit 
description: A helpful guide for those brand new to CTF, as I once was. 
image: "/assets/img/ctfaddict.png"


categories:
- CTF Guides

tags:
- misc
- rev
- foren
- crypto
- web
- pwn
- OSINT

date: 2025-7-1 00:00 -0500

# Intro 
Hello everyone! Today I will be talking about CTFs, what they are, and list and talk about different resources for getting better at them and practicing to win competitions.
This guide is based on learning from watching and competing in several CTF competitions. So, here's my take on all of this.

# What is CTF?
Capture the flags, more commonly known as CTFs, are cybersecurity challenges designed to give a user some context and information to be used to yield a series of random characters hidden inside of something,
otherwise known as a flag. Flags typically have what I call a header based on whatever competition it is. For example, for the writeups I did on BCACTF 2025, the flag format was
bcactf{flag}. 

# Why am I telling you about this? 
CTF competitions are fun to do if you're into networking or cybersecurity-related things, and even if you're not, you can learn a lot from them and have fun experiences with others.
The way I found out about them, my friend kinda asked me if I could be a member on his CTF team for a state-wide competition and we ended up winning, and he allowed me to be a permanent member on his team.
It's been a great experience and even better with friends and money to win.

# Types of CTF Challenges
Not all CTFs are created equal. There are 7 major types, and I will break them all down into a method of understanding that makes sense. 

Cryptography - Focuses mainly on encryption and ciphers. Sometimes you'll be breaking Caesar ciphers, other times you'll be dealing with weird XOR ciphers 
and modular math. Except for using a lot of decrypting tools and learning Python for scripts. Prepare for expertise on ciphers and decryption techniques.

Forensics - Consists heavily of file analysis of images, audio, and PCAPs to extract hidden data within them.
There are also other methods of extracting info that you will learn, including hex editors and metadata commands in Windows/Linux.

Web Exploitation - All about searching for and finding vulnerabilities in web pages and sites, such as SSTI injections,
cookie twisting, and login bypass methods. 

Reverse Engineering - This concerns a file or program you're typically given (.bin or .exe), and you have to figure out how it works without the source code. It's literally
what it's called: It's reversing a puzzle. Sometimes, the flag is within the logic, most times deeper. 

Binary Exploitation - This is typically called pwn, gaming jargon for hacker. Advanced stuff like buffer overflows or memory corruption to disrupt a program's behavior
One of the hardest categories in my opinion, due to it being advanced and Linux-based. 

Miscellaneous - This category is completely random, but consists of mainly of general skills. Every serious CTF competitor should know
a decent amount of misc challenges and how to solve them. 

OSINT - Short for Open Source Intelligence. You're given very little and have to go on an internet investigation to find the flag. Kinda related to rev, but doesn't solely focus on one file or
piece of information. It's ethical digital stalking basically. 

Alright, we've covered what CTFs are, why they are fun, and the different types of challenges. Next, tools and resources.

# Ultimate CTF Guide: Tools, Sites, and Applications.
For practicing CTFs, the first major website I can recommend to you is picoCTF. This site was developed by students at Carnegie Mellon, and it's a
great resource for practicing CTF challenges at all different levels, from basic beginner commands to advanced SQL injections. You can register in middle or high school and join a team. 

image: "/assets/img/pico.png"

Another CTF resource that covers a wide range of areas and difficulty levels is TryHackMe, which I think is right up there with Pico. I really like some of their challenges and they have great ways of teaching.
Hack the Box is also a pretty good one, but I would reserve this for more advanced CTF people, because this website heavily involves cybersecurity. 

Here are all the sources for each category for learning and some for doing:

Crypto - CyberChef, Dcode.fr, CryptoHack, CTF101, CrackStation, and various other cipher websites.
Foren - CTF101, Binary Ninja, Autopsy, Volatility, Binwalk, MorseDecoder, and Audacity.
Pwn - CryptoCat, PwnCollege, Nightmare, and CTF101.
Web - PortSwigger Labs, CTF101, picoCTF, and TryHackMe
Rev - Binary Ninja, Hack the Box, Objection, and CTF 101.
OSINT - Google or Bing is quite literally all you need generally.
Misc - Whatever the challenges require. 

# TIPS
- Practice at least 1 CTF a day if you can.
- Create a team to compete. Teams are the best way to grow and improve.
- For teams, divide the specialties—for example, 7 major categories, 6 that require actual improvement. For 3-person teams, assign one person to manage two main categories.
- CTFtime is the best website to find upcoming compeititons and you and your teammates can sign up under your team.
- I've been doing them for about 6 months, and it's been a good journey to track my improvement. It takes about a year to a year and a half to be really good, so be patient.

Well, that's all for now. Gonna try and lock in and post more, at least once a week. Thanks for reading
