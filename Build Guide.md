---
layout: page
title: Build Guide
permalink: /build-guide/
nav_order: 3
---
# Build Guide

Welcome to the build guide. This guide will go through building a Blue Team Pad from scratch. If yours is already built skip straight to the [usage guide](/blue-team-pad-docs/usage-guide/). If you need to source these parts visit the [ordering guide](/blue-team-pad-docs/ordering-guide/)

If you need to make any image bigger, right click on it and select `Open Image in New Tab`. This will open the image in a new tab and allow you to zoom in on it.

{: .warning }
Building the Blue Team Pad from scratch requires soldering!

## Part Overview

You should have the following parts before you start the build:

![Parts Image 1](/blue-team-pad-docs/images/part-overview-1.png){: width="800" }

![Parts Image 2](/blue-team-pad-docs/images/part-overview-2.png){: width="800" }

![Parts Image 3](/images/oled-socket.png){: width="400" }

## Parts List

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
16. 1x OLED Socket (Optional)


## Tool Overview

You will need the following tools to complete the build:

1. Soldering Iron
2. Solder (Lead Preferred)
3. 2 Pairs of Metal Tweezers or 2 Paperclips
4. 1.5mm Hex Screw Driver or allan key
5. 1 USB Type C Cable
6. Computer that can run VIAL

## Step 1: Testing the PCB & OLED

Before we do anything, we want to make sure our PCB & OLED is working as expected. Launch VIAL on your PC and connect the PCB.

{: .note }
If the Blue Team Pad is not recognized within VIAL, or shows up as a USB storage device named `RPI-RP2` you may need to flash the firmware on the device. To do so visit the [Flashing Guide](/blue-team-pad-docs/usage-guide/download-&-flash-firmware/)

Once connected Navigate to the `Matrix Tester` Tab within VIAL and click the `Unlock Keyboard` button in the bottom right.

Now, since the pad is not built, we will need to use our metal tweezers / paperclips to short the two unlock connections. This process can be done by shorting both the `SW23` and `SW19` pads at the same time until the bar fills on VIAL:

![Unlock PCB](/blue-team-pad-docs/images/unlock-pcb.jpeg){: width="800" }

![Unlock Bar](/blue-team-pad-docs/images/unlock-vial.png){: width="400" }

Once unlocked, use your pair of tweezers / paperclip to short each switch pad on the PCB.

![Test PCB](/blue-team-pad-docs/images/test-pcb.jpeg){: width="400" }

Then short the 2 pads corresponding to the switch for each encoder.  
These will be the 2 pins closest to the `SW2` & `SW3` markings on the PCB:

![Test Encoder Switch](/blue-team-pad-docs/images/test-encoder-switch.png){: width="400" }

If your PCB is fully functional, every key should be blue on VIAL as shown below:

![PCB Good](/blue-team-pad-docs/images/pcb-good-vial.png){: width="500" }


To test the OLED, first unplug the PCB from your PC. Then place the OLED within it's footprint on the top of the PCB as shown below so the pins make contact with the pads. Then plug the PCB back in. The OLED should light up and display Layer information as well as the name of the pad:

![OLED Test](/blue-team-pad-docs/images/oled-test.jpg){: width="600" }

## Step 2: Soldering Hot Swap Sockets

Now that we have all of our tools, parts & the PCB is tested we can begin the build.

First we will solder the hot swap sockets to the PCB.

Set up your solder iron and gather the PCB & 20x hot swap sockets.

One at a time place & solder each hot swap sockets within the designated areas on the pcb. These areas are marked `SW4` through `SW23`

{: .warning }
Ensure that your sockets are facing the correct direction! The pads will still line up if the part is flipped upside down! Refer to the photo below as a reference.

![Hot Swap Socket Direction](/blue-team-pad-docs/images/hs-socket-direction.png){: width="800" }

When soldering the sockets, ensure that each one is flush with the PCB as seen below:

![Flush Socket](/blue-team-pad-docs/images/flush-socket.jpg){: width="700" }

When you are finished soldering the sockets, your PCB should look like the following:

![Sockets Soldered](/blue-team-pad-docs/images/sockets-soldered.png){: width="600" }

## Step 3: Soldering Encoders

Next we will solder the two encoders to the PCB.

Line up each encoder and fit the pins within the `ENC 0` and `ENC 1` footprints on the PCB.

{: .note }
These will be soldered on the OPPOSITE side of the PCB compared to the hot swap sockets. Also ensure the encoders are flush before soldering them!

![Encoder Position](/blue-team-pad-docs/images/encoder-pos.jpg){: width="600" }

While the 2 larger "pins" do not carry any electrical current, they serve as a way to stabilize the encoder on the PCB, so be sure to solder them.

Once done your encoders' solder joints should look like the following:

![Encoder Pads Soldered](/blue-team-pad-docs/images/encoder-pads-soldered.jpg){: width="600" }

## Step 4: Assemble The Case

First, gather the following case parts:

* 1x Case Mid Piece (The one without the USB cutout!)
* 1x Plate
* 20x MX Switches

First line up the mid piece with the PCB as shown below:

![Case Mid Piece](/blue-team-pad-docs/images/case-mid-piece.jpg){: width="600" }

{: .note }
All of the case parts are NOT a perfect square, so you may need to rotate them to in order for the holes to line up.

Next grab the place and inset a few switches into the plate. Be SURE that the switches are inserted into the plate in the correct orientation.

The little rectangle on top of the plate must be on the left side, and the switches must be south facing. By south facing we want the LED hole to be facing south and the branding to be facing north. See the photo below for reference:

![Plate Orientation](/blue-team-pad-docs/images/plate-orientation.jpg){: width="600" }

{: .warning }
You must ensure that your switch pins are not bent! If they are bent, the switches will not fit into the hot swap sockets properly and this will prevent the switch in question from working.

Refer to the photo below for reference:

![Pin Direction](/blue-team-pad-docs/images/pin-direction.jpg){: width="700" }

Next, place the plate on top of the mid piece & pcb while simultaneously inserting the switches into the hot swap sockets. Be sure to line up the holes on the plate with the holes on the mid piece.

Be sure that once inserting the switches they are flush with the plate as shown below:

![Switches Flush](/blue-team-pad-docs/images/switches-flush.jpg){: width="600" }

Then Insert the rest of the switches, once again be sure to check every switch for bent pins!

![Switches Inserted](/blue-team-pad-docs/images/all-switches-in.jpg){: width="600" }

Once all of the switches are inserted, double check one last time to ensure that all of the switches are inserted correctly.

![Total Switches Flush](/blue-team-pad-docs/images/total-switches-flush.jpg){: width="600" }

## Step 5: Soldering the OLED (no socket)

{: .warning }
If you chose purchase the OLED sockets, skip to step 5.1

Before we solder our OLED, lets install the OLED cover. This will help protect the OLED from damage after installation.

First remove the protective film from the OLED. in this case it looks like a screen protector with a green pull tab.

![OLED Screen Protector](/blue-team-pad-docs/images/oled-screen-protector.jpg){: width="600" }

{: .warning }
Be sure to install the OLED cover with the correct orientation! If installed incorrectly, the OLED CAN be damaged! (2 OLEDs were broken in the process of prototyping this part)

If you look at the inside of the OLED cover closely, you will notice that the inside of one side of the cover has a small notch. This notch is meant for extra space for the ribbon cable that connects the OLED to it's PCB.

![OLED Cover Notch](/blue-team-pad-docs/images/oled-cover-notch.jpg){: width="600" }

Then place the OLED into the OLED cover by first inserting the side without pins into the cover so the ribbon cable slots into the aforementioned notch:

![OLED Cover Insert](/blue-team-pad-docs/images/oled-cover-insert.jpg){: width="600" }

Then press the side with the pins into the cover. It should fit snugly.

![OLED Cover Insert 2](/blue-team-pad-docs/images/oled-cover-insert-2.jpg){: width="600" }

Then insert the OLED through the plate so the pins fit into the PCB as shown below:

![OLED Insert](/blue-team-pad-docs/images/oled-insert.jpg){: width="600" }

Then solder the 4 OLED pins to the PCB as shown below:

![OLED Solder](/blue-team-pad-docs/images/oled-solder.jpg){: width="600" }


## Step 5.1: Soldering the OLED (socket)
{: .warning }
Be sure to install the OLED cover with the correct orientation! If installed incorrectly, the OLED CAN be damaged! (2 OLEDs were broken in the process of prototyping this part)

If you look at the inside of the OLED cover closely, you will notice that the inside of one side of the cover has a small notch. This notch is meant for extra space for the ribbon cable that connects the OLED to it's PCB.

![OLED Cover Notch](/blue-team-pad-docs/images/oled-cover-socket.png){: width="600" }

Then install the socket on the OLED by pressing it into the socket as shown below:

![OLED In Socket](/blue-team-pad-docs/images/oled-in-socket.png){: width="600" }


Then place the OLED into the OLED cover by first inserting the side without pins into the cover so the ribbon cable slots into the aforementioned notch:

![Put OLED In Socket](/blue-team-pad-docs/images/put-oled-in-cover-socket.png){: width="600" }

Then press the side with the pins into the cover. It should fit snugly.

![OLED Cover In Socket](/blue-team-pad-docs/images/oled-in-cover-socket.png){: width="600" }

Then insert the OLED with the socket attached through the plate so the pins fit into the PCB as shown below:

![OLED Socket Installed](/blue-team-pad-docs/images/oled-cover-socket-installed.png)

Then solder the 4 OLED pins to the PCB as shown below:

![OLED Solder](/blue-team-pad-docs/images/oled-solder.jpg){: width="600" }

## Step 6 Testing the OLED & Switches

Now that all of the electronics are assembled we can check to make sure everything is working properly.

First, plug in the macro pad into your computer and connect it to VIAL.

The OLED should light up and display the current layer and `Blue Team Pad`.

![OLED Working](/blue-team-pad-docs/images/oled-working.jpg){: width="600" }

{: .note }
The OLED will go into sleep mode after ~60 seconds of inactivity. To wake it up, press any key on the pad. This is to prevent OLED burn-in.

Then just how we first tested the pcb, navigate to the matrix tab, unlock the Pad, and press each switch to ensure that they are working properly.

Every switch should light up when you push it. If a switch does not, remove it and check the pins to ensure that they are not bent.

![Switches Working](/blue-team-pad-docs/images/pcb-good-vial.png){: width="600" }

## Step 7: Finish Case Assembly

Now that we have confirmed that the electronics are working properly, we can finish assembling the case.

First, grab the 4x m2x16mm screws and insert them through each hole in the corners of the plate as shown below:

![Screws Inserted](/blue-team-pad-docs/images/screws-inserted.jpg){: width="600" }

{: .note }
You may have to use your screwdriver to "screw" your screws through the 3d printed parts during assembly, this is by design to ensure a snug case assembly.

Then grab the mid piece with the USB cutout and place it on the PCB, screwing it into the 4 screws.

You will notice that there is a small notch on this part, Be sure to line that notch up with `R6` on the PCB as shown below:

![Mid Piece Notch](/blue-team-pad-docs/images/mid-piece-notch.jpg){: width="600" }

The mid piece should look like the following once installed:

![Mid Piece Screwed](/blue-team-pad-docs/images/mid-piece-screwed.jpg){: width="600" }

First, insert the 4 M2 nuts into each nut hole on the bottom piece as shown below:

![Bottom Piece Nuts](/blue-team-pad-docs/images/bottom-piece-nuts.jpg){: width="600" }

Next grab the bottom piece and screw it on to the USB mid piece as shown below. The thicker part of the bottom piece should be facing the USB cutout.

![Bottom Piece Installed](/blue-team-pad-docs/images/bottom-piece-installed.jpg){: width="600" }

Then, install the 4 rubber bumpons in the 4 holes on the bottom piece as shown below:

![Bumpons Installed](/blue-team-pad-docs/images/bumpons-installed.jpg){: width="600" }

Next, grab the 2 knobs and press-fit them onto the encoders. These are a tight fit, so you may need to use a bit of force.

![Knobs Installed](/blue-team-pad-docs/images/knobs-installed.jpg){: width="600" }

Finally, install your key caps of choice by press-fitting them onto the top of the switches!

![Fully Assembled](/blue-team-pad-docs/images/fully-assembled.jpg){: width="600" }

That's it! You have now successfully assembled your Blue Team Pad!
