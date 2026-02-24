---
title: Static URL
aliases:
- "/docs/gitlabupdater"
---

### URL

Link to a static url to a file, like so:

`https://example.com/downloads/latest.appimage`

This is a valid example for the app Beeper:

`https://api.beeper.com/desktop/download/linux/x64/stable/com.automattic.beeper.desktop`


#### Requirements

In order for a link to be valid, Gear Lever performs the following checks:

1. The web server must support the HEAD method
2. The server must return a `Size` header
3. The `Size` of the new file must be different from the size of the currently instelled file, 
    this is how Gear Lever determines if there is a new release or not.
4. The `Content-Type` of the file must be one of the followings:

```
application/x-iso9660-appimage
application/vnd.appimage
application/x-appimage
binary/octet-stream
application/octet-stream
```