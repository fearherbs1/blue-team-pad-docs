---
layout: page
title: Ordering Guide
permalink: /ordering-guide/
nav_order: 2
---
# Ordering Guide

This page will guide you through the process of ordering all of the parts you need to build you own BlueTeamPad.

## Parts List

Below is the parts list. Links & prices are current as of April 2023. Note that some parts have a MOQ (minimum order quantity), so you may need to order more than you need. The prices include the minimum you must purchase. Given that the PCB MOQ is 5 and many other MOQs are quite high, I would recommend building 5 units and selling / giving away the extras.

### The absolute minimum spend for one unit is $135.62

(All Prices Are In USD)

| Part Name                           | Part # (If Applicable) | \# Needed for 1 Unit | MOQ | \# Needed Due To MOQ | Total Cost (No Shipping) | Link                                                                                                                                                                                                                                                                   |
| ----------------------------------- | ----------------------- | -------------------- | --- | -------------------- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PCB + Assembly                      |                         | 1                    | 5   | 5                    | $34.06                   | [JLCPCB](https://jlcpcb.com/)                                                                                                                                                                                                                             |
| JWICK Black (MX Switches)           |                         | 20                   | 18  | 36                   | $8.28                    | [Divinikey](https://divinikey.com/products/jwk-jwick-linear-switches)                                                                                                                                                   |
| 3D Printing Spool (Self Print Only) |                         | 1                    | 1   | 1                    | $24.99                   | [Amazon](https://www.amazon.com/HATCHBOX-3D-Filament-Dimensional-Accuracy/dp/B00J0ECR5I/)                                                                                                     |
| Kailh MX Hot Swap Sockets           | CPG151101S11            | 20                   | 50  | 50                   | $7.50                    | [AliExpress](https://www.aliexpress.us/item/2255800865526224.html) |
| Relegendable Keycaps (MX Style)     |                         | 20                   | 10  | 20                   | $4.08                    | [AliExpress](https://www.aliexpress.us/item/3256803271770916.html) |
| OLEDs (4 pin IC2 .91in)             | SSD1306                 | 1                    | 5   | 5                    | $12.88                   | [Amazon](https://www.amazon.com/gp/product/B08ZY4YBHL/)                                                                           |
| USBC to A Cables                    |                         | 1                    | 2   | 2                    | $8.99                    | [Amazon](https://www.amazon.com/gp/product/B07DC5PPFV/)                                                                           |
| Bumpons (8mm Diameter) (2mm Thick)  |                         | 4                    | 100 | 100                  | $6.98                    | [Amazon](https://www.amazon.com/gp/product/B07DN6W6VN/)                                                                           |
| 16mm M2 Machine Screws              | 91290A047               | 4                    | 100 | 100                  | $13.03                   | [MCMaster](https://www.mcmaster.com/catalog/129/3494/91290A047)                                                                                                                                                             |
| M2 Nuts                             | 98676A310               | 4                    | 100 | 100                  | $11.38                   | [MCMaster](https://www.mcmaster.com/catalog/129/3585/98676A310)                                                                                                                                                             |
| Oled Sockets                        | C2718488                | 1                    | 10  | 10                   | $0.43                    | [LCSC](https://www.lcsc.com/product-detail/Female-Headers_BOOMELE-Boom-Precision-Elec-C2718488_C2718488.html)                                                         |
| Encoders                            | C255515                 | 2                    | 1   | 2                    | $3.02                    | [LCSC](https://www.lcsc.com/product-detail/Rotary-Encoders_ALPSALPINE-EC11E18244A5_C255515.html)     


## Ordering The PCB

While ordering all of the other parts is self explanatory, the PCB is a bit more complicated. The PCB is designed to be assembled by JLCPCB.

First navigate to the [JLCPCB](https://jlcpcb.com/) website. Then click on the "PCB Assembly" tab. Then click on the PCB Assembly "Get Quote" button. It should bring you to a page that looks like this:

![JLCPCB Assembly Page](/blue-team-pad-docs/images/JLCPCB-Assembly-page.png)

Next download the the following files from the [BlueTeamPad Github Releases Page](https://github.com/fearherbs1/blue-team-pad/releases/tag/v1.1)

* GERBER-BlueTeamPad.zip
* POS-BlueTeamPad.csv
* BOM-BlueTeamPad.csv

Then Click the `Add Gerber File` and upload the `GERBER-BlueTeamPad.zip`.

Once uploaded select the following options:  
(Most of this should be auto populated)

* Base Material: FR4
* Layers: 2
* Dimensions: 103.19mm x 107.16mm
* PCB Quantity: 5
* Product type: Industrial/Consumer Electronics
* Different Design: 1
* Delivery Format: Single PCB
* PCB Thickness: 1.6mm
* PCB Color: Black (Or What Ever Color You Want)
* Silkscreen Color: White
* Surface Finish: HASL(With Lead)
* Outer Copper Weight: 1oz
* Via Covering: Tented
* Confirm Production File: Yes
* Remove Order Number: Specify a location
* Flying Probe Test: Fully Test
* Gold Fingers: No
* Castellated Holes: No

Then add the PCB Assembly Options:

* PCBA Type: Economic
* Assembly side: Bottom Side
* PCBA Quantity: 5
* Tooling Holes: Added by JLCPCB
* Confirm Parts Placement: Yes

Then on the next page you will be greeted with the following screen:

![BOM/POS Page](/blue-team-pad-docs/images/bom-pos-jlcpcb.png)

Download the `BOM-BlueTeamPad.csv` file [Here](https://github.com/fearherbs1/blue-team-pad/releases) and upload it using the `Add Bom File` button.

Then download the `POS-BlueTeamPad.csv` file [Here](https://github.com/fearherbs1/blue-team-pad/releases) and upload it using the `Add CPL File` button.

After clicking next, *ensure that all of the parts are in stock*. It should look something like the page below.

![BOM All Parts](/blue-team-pad-docs/images/BOM-ALL-Parts.png)

Then on the next page you can see a 3d rendering of all of the parts on the pcb.

![PCB 3D Rendering](/blue-team-pad-docs/images/pcb-3d-rendering.png)

Click next, you should be all set, but if there are any issues with parts placement a JLCPBC engineer will correct the placement and send you an email.

After that you can add the order to your cart and checkout.

## 3d Printed Parts

If possible, I highly recommend printing the parts yourself or visiting a local maker space for access to a 3d printer. If you cannot get access to one JLCPCB also has a 3d printing service but from what I have seen it is quite expensive.

If you plan to print the parts yourself, the STL files are available on the [BlueTeamPad Github Releases Page](https://github.com/fearherbs1/blue-team-pad/releases) in a file named `Case.STLs.zip`.

### Print Settings

I used the following settings when printing the parts:

* Layer Height: 0.2mm
* Infill: 15%
* Supports: No
* Material: PLA


