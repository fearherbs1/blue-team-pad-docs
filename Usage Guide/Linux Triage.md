---
layout: default
title: Linux Triage
nav_order: 4
parent: Example Macros
grand_parent: Usage Guide
permalink: /usage-guide/example-macros/linux-triage
---

# Linux Triage:

## Show all processes & locations

This shows all processes and their source executables.

```json
[["text", "ps aux"]]
```

## Forcefully end process

Force end a process.

```json
[["text", "kill -9 <pid>"]]
```

## Show systemd services

Show all systemd services on the system.

```json
[["text", "ls -la /etc/systemd/system/*.service"]]
```

## Show non-systemd services

```json
[["text", "ls -la /etc/init.d/"]]
```

## Show crontabs

Show all crontabs on the system.

```json
[["text", "ls -la /etc/cron*; ls -la /var/spool/cron/*"]]
```

## Show at jobs

Show all "at" jobs on the system

```json
[["text", "ls -la /etc/cron*; ls -la /var/spool/cron/*"]]
```
