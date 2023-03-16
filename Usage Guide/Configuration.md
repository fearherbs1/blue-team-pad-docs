---
layout: page
title: Configuration
nav_order: 2
parent: Usage Guide
permalink: /usage-guide/configuration/
---

# Configuration

In order to configure the device we have two options, VIAL Web & the VIAL App. The one you use is completely up to you as they both have the same functionality.

VIAL web is very useful if you are in a situation where installing programs on your computer is not possible, such as corporate devices as everything is done through a web browser.  

Though, if you are allowed to download programs I recommend the downloadable app instead.

## VIAL Web

To configure the device using VIAL web, just click the button below:

[Launch Vial Web](https://vial.rocks/){: .btn .btn-blue }

{: .warning }
In order to use this method, you must be using a browser that supports `WEB HID`. As of writing, only Chrome, Opera & Edge support this protocol. You can check up to date browser support [Here](https://caniuse.com/webhid).

Once on the site click the `Start Vial` button as shown below:

![Start Vial](/blue-team-pad-docs/images/start-vial.png)

This will prompt you to authorize a device to be used.  

Click the entry for `blue_team_pad` and then click connect:

![Connect to Vial Web](/blue-team-pad-docs/images/connect-to-vial-web.png)


After a few seconds your device will then connect and be ready for configuration!

![Ready To Configure](https://fearherbs1.github.io/blue-team-pad-docs/images/vial-web-connected.png)

## VIAL App

First download and install the VIAL app for your operating system:

[Download VIAL](https://get.vial.today/download/){: .btn .btn-blue }

{: .warning }
Linux Users May need to create a custom `udev` rule in order for the device to show up within the VIAL App. You can read how to do this within the VIAL documentation [HERE](https://get.vial.today/manual/linux-udev.html)

Then launch the app, your device should show up within the menu at the top and be ready to configure!

![Vial App Ready](https://fearherbs1.github.io/blue-team-pad-docs/images/vial-app-ready.png)
