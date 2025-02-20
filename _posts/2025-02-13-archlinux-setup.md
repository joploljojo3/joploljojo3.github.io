---
layout: post
title:  "Arch linux installation"
date:   2025-02-13 14:34:00 +0100
categories: jekyll update
---

# Hello again!
Welcome back! today we'll be taking a look at how i went about installing arch linux in a vm.

# Index:

1. [Installation](#1-installation)
2. [Setup](#2-setup)

# 1. Installation
The installation was a bit rocky, but i got through it. here's some stuff i encountered.

1) EFI vs BIOS:

One of the installation steps required me to install a bootloader. I chose to use [GRUB](https://en.wikipedia.org/wiki/GNU_GRUB), mostly because i'm already a bit familiar with it. Going through the installation of grub didn't work, because i was using a BIOS system, while the installation apparently required an EFI system. after changing this out in VirtualBox, the installation worked as usual. Immediately after doing the grub installation, I scrolled down and found the BIOS installation guide.

2) grub-mkconfig

Due to not reading the installation guide fully, I read over the part where it said you must use `grub-mkconfig` before you reboot, so i had to boot into the installer again to fix that.

# 2. Setup
The setup was fun! i learnt a lot about linux, surprisingly. Here's some notable stuff that happened:

- Had to configure my ethernet connection manually
- sudo not installed
- vim / nano not installed. (which made the first one more difficult too)
- dhcpcd not installed
- ssh keys not working (still not fixed)

