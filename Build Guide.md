---
layout: page
title: Build Guide
permalink: /build-guide/
nav_order: 3
---
# Build Guide

Welcome to the build guide. This guide will go through building a Blue Team Pad from scratch. If yours is already built skip straight to the [usage guide](https://fearherbs1.github.io/blue-team-pad-docs/usage-guide/). If you need to source these parts visit the [ordering guide](https://fearherbs1.github.io/blue-team-pad-docs/ordering-guide/)

{: .warning }
Building the Blue Team Pad from scratch requires soldering!

## Part Overview

You should have the following parts before you start the build:

![Parts Image 1](/images/part-overview-1.png){: width="800" }

![Parts Image 2](/images/part-overview-2.png){: width="800" }

## Parts List:


1. 20 MX Style Switches of Your Choice
2. 1x Plate
3. 1x PCB
4. 1x Case Mid Piece
5. 1x Case Bottom Piece
6. 2x Knobs
7. 2x EC11 Encoders [LCSC Link](https://www.lcsc.com/product-detail/Rotary-Encoders_ALPSALPINE-EC11E18244A5_C255515.html)
8. 20x Kalith or Gataron MX Hotswap Sockets
9. 4x Rubber Bumpons (8mm Diameter)
10. 1x OLED
11. 4x M2 Machine Screws (16mm)
12. 4x M2 Nuts
13. 20 Keycaps of Your Choice
14. 1x Case USB Mid Piece
15. 1x OLED Cover


## Tool Overview

You will need the following tools to complete the build:

1. Soldering Iron
2. Solder (Lead Preferred)
3. 2 Pairs of Metal Tweezers or 2 Paperclips
4. 1.5mm Hex Screw Driver or allan key
5. 1 USB Type C Cable
6. Computer that can run VIAL

## Step 1: Testing the PCB

Before we do anything, we want to make sure our PCB is working as expected. Launch VIAL on your PC and connect the PCB.

{: .note }
If the Blue Team Pad is not recognized within VIAL, or shows up as a USB storage device named `RPI-RP2` you may need to flash the firmware on the device. To do so visit the [Flashing Guide](/usage-guide/download-&-flash-firmware/)

Once connected Navigate to the `Matrix Tester` Tab within VIAL and click the `Unlock Keyboard` button in the bottom right.

Now, since the pad is not built, we will need to use our metal tweezers / paperclips to short the two unlock connections. This process can be done by shorting both the `SW23` and `SW19` pads at the same time until the bar fills on VIAL:

![Unlock PCB](/images/unlock-pcb.jpeg){: width="800" }



## Step 2: Soldering Hot Swap Sockets

Now that we have all of our tools & parts we can begin the build.

First we will solder the hot swap sockets to the PCB.

Set your solder iron and gather the PCB & 20x hot swap sockets.

One at a time place & solder each hot swap sockets within the designated areas on the pcb. These areas are marked `SW4` through `SW23`