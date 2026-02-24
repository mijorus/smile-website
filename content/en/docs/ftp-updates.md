---
title: FTP Updates
aliases:
- "/docs/ftpupdater"
---

The following shows how to configure an app to use Github as the update source, for Gear Lever 4.+.

Let's use https://www.digikam.org/download as an example.

[This page](https://download.kde.org/stable/digikam/8.8.0/digiKam-8.8.0-Qt6-x86-64.appimage.mirrorlist)
lists all the available FTP servers for Digikam. Let's pick the best one for current our location.

(Files for Digikam are exposed under http and ftp);

`https://mirror.gofoss.xyz/kde-ftp/stable/digikam/8.8.0/digiKam-8.8.0-Qt6-x86-64.appimage`

### Server URL

FTP servers must start with `ftp://`

`ftp://mirror.gofoss.xyz`

### File path

`kde-ftp/stable/digikam/*/digiKam-*-Qt6-x86-64.appimage`