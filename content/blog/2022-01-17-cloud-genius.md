---
title: "Cloud Genius, VIM, and fish"
description: "Customizing EndeavourOS"
date: "2022-01-17"
utterances_term: "Untitled"
categories: [linux]
---
### Cloud Genius, VIM, and fish
> Customizing EndeavourOS

#### Cloud Genius
Today kicked off [Cloud Genius](https://cloudgenius.app/) He puts on a free (for veterans)  platform
agnostic cloud training platform with an emphasis on open source and using the command line.
Day 1 covered some basics such as public/private key pairs, the definition of cloud, the types of cloud
,etc.

He wrote a lot of scripts for ubuntu to automatically provision a custom AWS EC2 instance,and to automatically
install needed software for the local development environment. I took it on as a challenge to just wget
the scripts, read through them line by line and convert them into commands that would work on arch.
For example `apt-get install foo` become `pacman -S foo` for arch. no biggie. good practice.

#### Linux

Seems like I mostly just tinkered with linux today. I also dug into the fish config a little bit and
made my terminal just a bit more useful by adding git status symbols to the prompt. Small change,
big impact. Also committed to learning vim a little more. Fun fact of the day...\*nix has TWO clipboards
woah. VIM wise, learned how to easily select whole lines with visual or visual line mode, then yank
*(such a better word than copy)* with `y` and paste with `middlemouse`. Strange, but I'll adapt.

#### Coding

I made some more headway on the data structures and algo course and managed to implement a divide
and conquer aka binary search method. My logic was convoluted compared to what the instructor provided,
but refinement comes with repetition. I also did some light reading on generics, which is a concept
that basically doesn't exist in JavaScript but exists in most strongly typed languages. I think
my coding vocabulary is reaching a good point, but I'm sure that feeling will go away once I try
to learn another language.

