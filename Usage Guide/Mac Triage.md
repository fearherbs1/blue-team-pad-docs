---
layout: default
title: Mac Triage
nav_order: 3
parent: Example Macros
grand_parent: Usage Guide
permalink: /usage-guide/example-macros/mac-triage/
---

# Mac Triage:

## List Users

List Users on the system

```json
[["text", "dscl . list /Users"]]
```

## List Groups

List Groups on the system

```json
[["text", "dscl . list /Groups"]]
```

## List Crontabs

List out the crontab locations

```json
[["text", "sudo ls -la /usr/lib/cron/tabs; sudo ls -la /var/at/tabs"]]

```

## Get Detailed Metadata About a file

Sometimes you can use this to get where a file was downloaded from

```json
[["text", "mdls '<filePath>'"]]
```

## Show all processes & locations

```json
[["text", "ps aux"]]
```

## Get all launch agents and their corresponding plist files

Obtain all launch agents and the files they originate from.

```json
[["text", "find /System/Library/Launch* /Library/Launch* /Users/*/Library/Launch* -name '*.plist' -print -exec /usr/libexec/PlistBuddy -c \"Print Label\" {} ';'"]]
```