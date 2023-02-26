---
layout: default
title: Windows Triage
nav_order: 2
parent: Example Macros
grand_parent: Usage Guide
permalink: /usage-guide/example-macros/windows-triage
---

# Windows Triage:

All of the following macros are Powershell based.

## View System & User Run Key

Get startup values stored in the System & User Run keys

```json
[["text", "gi registry::HKLM\\Software\\Microsoft\\Windows\\CurrentVersion\\Run; gi registry::HKCU\\Software\\Microsoft\\Windows\\CurrentVersion\\Run"]]

```

## Running Processes

List all running processes, their pid, and source path.

```json
[["text", "Get-Process | Select-Object ID,NAME,PATH"]]
```

## Get .lnk File Target

Get's the target file of a .lnk / shortcut file. You must replace `<Full-Path-To-LNK-File>` with the full path to the lnk file in question.

```json
[["text", "$sh = New-Object -ComObject WScript.Shell;$target = $sh.CreateShortcut('<Full-Path-To-LNK-File>').TargetPath; $target | Out-String"]]

```

## Get Contents of All user's Startup Folders

This will list out all items in every user's startup folder.

```json
[["text", "gci \"C:\\Users\\*\\AppData\\Roaming\\Microsoft\\Windows\\Start Menu\\Programs\\Startup\" -R -Force"]]

```

## Get all Scheduled Tasks calling a `.exe` file:

```json
[["text", "Get-ScheduledTask | Select-Object -Property Taskname,Taskpath -ExpandProperty Actions | Where-Object {$_.Execute -like '*.exe'} | Select-Object Taskname,Taskpath,Execute,Arguments | Format-List | Out-String"]]

```

## Search All User Folders for a given term

After using this macro, append your search term to the end of the command.  

For example: `gci -Path $Env:SystemDrive\\Users\\*\\ -R -ea 0 -Fo -In BadFileName`

```json
[["text", "gci -Path $Env:SystemDrive\\Users\\*\\ -R -ea 0 -Fo -In "]]
```

## Get Windows Services & Paths

Get all of the services on a windows system along with state & executable path.

```json
[["text", "Get-WmiObject win32_service | select Name, DisplayName, State, PathName"]]

```

## Get Zone Identifier

This can be used to see where a file was downloaded from.

```json
[["text", "Get-Content -Path <filepath> -Stream zone.identifier"]]
```
