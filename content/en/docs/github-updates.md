---
title: Github Updates
aliases:
- "/docs/githubupdater"
---

## Using the GUI

The following shows how to configure an app to use Github as the update source, for Gear Lever 4.+.

Let's use https://github.com/VSCodium/vscodium as an example.

### Repo URL
This should be the URL of the repo, without addiitonal parameters:

`https://github.com/VSCodium/vscodium`


### Release file name
This should be the name of the file from the relases tab; you can use globe (*) patterns to indicate variables
in the file name.

`VSCodium-*-x86_64.AppImage`

Pay attention as may apps today have relases for x86_64 and arm64 platforms.


### Allow pre-releasese

I/O switch to enable update pre-releases: some apps might release new versions flagged 
as "drafts", which will be ignored when this flag is OFF.