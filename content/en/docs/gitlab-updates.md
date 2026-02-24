---
title: Gitlab Updates
aliases:
- "/docs/gitlabupdater"
---
The following shows how to configure an app to use Gitlab as the update source, for Gear Lever 4.+.
Please not that **custom Gitlab instances are not supported** fot the time being.

Let's use https://gitlab.com/librewolf-community/browser/appimage as an example.

### Repo URL
This should be the URL of the repo, without addiitonal parameters:

`https://gitlab.com/librewolf-community/browser/appimage`


### Release file name
This should be the name of the file from the relases tab; you can use globe (*) patterns to indicate variables
in the file name.

`LibreWolf-*.x86_64.AppImage`

Pay attention as may apps today have relases for x86_64 and arm64 platforms.