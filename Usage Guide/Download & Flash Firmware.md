---
layout: page
title: Download & Flash Firmware
nav_order: 1
parent: Usage Guide
permalink: /usage-guide/download-&-flash-firmware/
---

# Flashing Guide

While the blue team pad is compatible with four different firmware variants, it is recommended to use VIAL for maximum functionality. Due to this, we will focus on VIAL usage throughout this guide.

{: .warning }
While the PCB does come pre-flashed with VIAL, it is recommend to re-flash the device once you obtain it for security purposes.

## Download Firmware

Download the latest VIAL firmware by clicking the button below:

[Download VIAL Firmware](https://github.com/fearherbs1/blue-team-pad/releases/download/v1.1/fearherbs1_blue_team_pad_vial.uf2){: .btn .btn-blue }


For more firmware options visit the [Github Releases Page](https://github.com/fearherbs1/blue-team-pad/releases).

## Verify Download (Optional but recommended)

{: .warning }
The SHA-256 hash of the downloaded file should match the following value `B98B22DA1BE6B67B949F1CB15687DC896EB5381282549B97363BEBFC27F35975` If it does not, your download may have been tampered with!

You can check this value using the following commands:

Mac:

```zsh
shasum -a 256 fearherbs1_blue_team_pad_vial.uf2
```
Linux:

```bash
sha256sum fearherbs1_blue_team_pad_vial.uf2
```

Windows Powershell:

```powershell
get-filehash -Algorithm SHA256 .\fearherbs1_blue_team_pad_vial.uf2
```


## Flashing

Now that we have our firmware, we need to enter the boot-loader.

To do this, hold down the left knob and plug the device into your computer.

If no firmware is installed on the device, just plugging it in without holding any buttons will have the same effect.

If your knob is not soldered onto the board yet, shorting the two `BOOT` pins on the back side of the PCB will also have the same effect.

Once plugged in, the device will show as a storage device named `RPI-RP2`.

![](/images/flashing-storage-device.png)

To complete the flashing, copy the `fearherbs1_blue_team_pad_vial.uf2` file to the root of the `RPI-RP2` device.

Once the file transfers, the device will re-connect to the host computer ready to be used!

{: .note }
If you are attempting to flash the device on a mac, dragging & dropping the file over using Finder may fail. If this happens use the copy (`cp`) command within the terminal instead. Ex: `cp fearherbs1_blue_team_pad_vial.uf2  /Volumes/RPI-RP2`






