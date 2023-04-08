---
layout: page
title: Mac Info
nav_order: 5
parent: Usage Guide
permalink: /usage-guide/mac-info/
---
# Mac Info

## Modifier Keys

As you may already know, Macs use `command (⌘)` as their windows & linux `control` equivalent even though they still have a `control (⌃)` key. So, when a "windows" keyboard is used on a mac the keys act as follows by default:

* control --> control (^)
* windows Key (GUI) --> command (⌘)
* alt --> option (⌥)

While this does not pose any issue on its own, for maximum compatibility of macros across operating systems, it is recommended to rebind the modifier keys within mac `System Settings` app to the following:

![Mac Settings](/blue-team-pad-docs/images/mac-mods-settings.png){: width="700" }

Note that this only has to be done the first time you plug the macro pad into your Mac.

This menu can be reached by searching for `customize modifier keys` within the mac settings app and selecting the `blue_team_pad` from the dropdown menu.

Now if we create a simple macro to issue the copy command, we can save it as `LCTRL+C` and it will work on both operating systems.

If you were to program mac-specific macros after doing this change you would use:

* control as command (⌘)
* alt as option (⌥)
* Windows Key (GUI) as control (^)
