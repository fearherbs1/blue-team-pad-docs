---
layout: default
title: Productivity
nav_order: 1
parent: Example Macros
grand_parent: Usage Guide
permalink: /usage-guide/example-macros/productivity/
---

# Productivity

## Search VirusTotal

Search virus total for whatever is present in the system clipboard. Your active window must be a browser.

```json
[["down", "KC_LCTRL"], ["tap", "KC_T"], ["up", "KC_LCTRL"], ["text", "https://www.virustotal.com/gui/search/"], ["down", "KC_LCTRL"], ["tap", "KC_V"], ["up", "KC_LCTRL"], ["delay", 20], ["tap", "KC_ENTER"]]

```

## Google Translate

Translate whatever is present in the system clipboard using google translate. Your active window must be a browser.

```json
[["down", "KC_LCTRL"], ["tap", "KC_T"], ["up", "KC_LCTRL"], ["text", "https://translate.google.com/?sl=auto&tl=en&op=translate&text="], ["down", "KC_LCTRL"], ["tap", "KC_V"], ["up", "KC_LCTRL"], ["delay", 20], ["tap", "KC_ENTER"]]

```

## CyberChef

Enter the system clipboard into the cyberchef instance located at "https://gchq.github.io/CyberChef" Your active window must be a browser. You may need to adjust the delay if you have a slow internet connection. You can also edit the url with a commonly used recipe if you desire.

### Firefox:

```json
[["down", "KC_LCTRL"], ["tap", "KC_T"], ["up", "KC_LCTRL"], ["text", "https://gchq.github.io/CyberChef/"], ["tap", "KC_ENTER"], ["delay", 2000], ["tap", "KC_TAB"], ["down", "KC_LCTRL"], ["tap", "KC_V"], ["up", "KC_LCTRL"]]

```
### Chrome:

```json
[["down", "KC_LCTRL"], ["tap", "KC_T"], ["up", "KC_LCTRL"], ["text", "https://gchq.github.io/CyberChef/"], ["tap", "KC_ENTER"], ["delay", 2000], ["down", "KC_LSHIFT"], ["tap", "KC_TAB"], ["up", "KC_LSHIFT"], ["down", "KC_LCTRL"], ["tap", "KC_V"], ["up", "KC_LCTRL"]]

```

## Google Search

Search whatever is present in the system clipboard using google. Your active window must be a browser.

```json
[["down", "KC_LCTRL"], ["tap", "KC_T"], ["up", "KC_LCTRL"], ["text", "https://www.google.com/search?&q="], ["down", "KC_LCTRL"], ["tap", "KC_V"], ["up", "KC_LCTRL"], ["delay", 20], ["tap", "KC_ENTER"]]

```

## Fast Windows Shutdown

Shuts down a windows computer using the win + x method.

```json
[["down", "KC_LGUI"], ["tap", "KC_X"], ["up", "KC_LGUI"], ["delay", 20], ["tap", "KC_U"], ["tap", "KC_U"]]
```

## Launch Admin Powershell

Launches an Admin level Powershell Window. Automatically Accepts UAC Prompt. You may have to adjust the delay for slower computers.

```json
[["down", "KC_LGUI"], ["tap", "KC_R"], ["up", "KC_LGUI"], ["delay", 200], ["text", "powershell.exe"], ["delay", 20], ["down", "KC_LCTRL", "KC_LSHIFT"], ["tap", "KC_ENTER"], ["up", "KC_LCTRL", "KC_LSHIFT"], ["delay", 800], ["tap", "KC_LEFT"], ["tap", "KC_ENTER"]]

```
