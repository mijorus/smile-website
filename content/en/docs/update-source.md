---
title: Update source
---


## Using the CLI

For Gear Lever 4.2+.

The following documentation assumes that you created the following alias:

```sh
alias gearlever="flatpak run it.mijorus.gearlever"
```

### Get a list of all the available update managers

```sh
gearlever --list-update-managers
```

### Set an update source

```sh
gearlever \
--set-update-source <file_path> \
--manager GithubeUpdater \
  repo_url=<url> \
  repo_filename=<pattern> \
  allow_prereleases=<value> # Use 0 or 1, true or false, for boolean values
```

Variables change depending on the update manager, please check the
available variables using:

```sh
gearlever --set-update-source --manager <manager> --help
```
