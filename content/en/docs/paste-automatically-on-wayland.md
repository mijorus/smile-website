---
title: Paste automatically on Wayland
---


There are multiple options to paste the emojis automatically on Wayland.


## Option 1 (GNOME)

Use the GNOME extension, requires Smile 2.4.0 or greater.

<a href="https://extensions.gnome.org/extension/6096/smile-complementary-extension" align="center">
  <img width="200" src="https://raw.githubusercontent.com/mijorus/smile/refs/heads/master/docs/gnome-extension.svg">
</a>


## Option 2 (Should work for all desktop environments)

> [!WARNING]
> This solutions has security implications, as it may expose control to your input devices to malicious apps.
>
> If this is a concern for you, please don't follow this guide.
>
> (Granted, we have been using Xorg for years, which did not have these guidelines and we where fine with it)

Automatically paste content on other apps is not possibile on Wayland without an additional configuration.

Smile relies on [dotool](https://sr.ht/~geb/dotool/), which is way easier to set-up compared to alternatives like `ydotool`.

**Requires Smile 2.11.0**

### Step 1: install `dotool`

Packages are available for Arch and other system, read more here:
https://sr.ht/~geb/dotool/

1. Install requirements

```bash
# Ubuntu
sudo apt install go libxkbcommon-devel scdoc

# Fedora
sudo dnf install go libxkbcommon-devel scdoc
```

2. Build and install dotool

One-line solution:

```bash
curl -fsSL https://raw.githubusercontent.com/mijorus/smile/refs/heads/master/extras/install-dotool.sh | bash
```

3. Restart the computer

### Step 2: Install the `smile-autopaste.service`

One-line solution:

```bash
curl -fsSL https://raw.githubusercontent.com/mijorus/smile/refs/heads/master/extras/autopaste-service-install.sh | bash
```

To uninstall the service, if needed, run:

```
curl -fsSL https://raw.githubusercontent.com/mijorus/smile/refs/heads/master/extras/autopaste-service-uninstall.sh | bash
```

