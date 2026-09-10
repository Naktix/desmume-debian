# DeSmuME for Debian

This repository builds [DeSmuME](https://github.com/TASEmulators/desmume) as a native .deb package and publishes it on GitHub Pages.

## How to install

Add the signing key and repository:

```bash
curl -fsSL https://naktix.github.io/desmume-debian/desmume.gpg | sudo tee /etc/apt/keyrings/desmume.gpg > /dev/null

echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/desmume.gpg] https://naktix.github.io/desmume-debian trixie main" | sudo tee /etc/apt/sources.list.d/desmume.list
```

Update the package lists:

```bash
sudo apt update
```

Install DeSmuME:

```bash
sudo apt install desmume-gtk
```

## How to remove

Remove DeSmuME:

```bash
sudo apt remove desmume-gtk
```

Remove the repository and signing key:

```bash
sudo rm /etc/apt/sources.list.d/desmume.list

sudo rm /etc/apt/keyrings/desmume.gpg
```

Update the package lists:

```bash
sudo apt update
```

> **Disclaimer:** This is an unofficial repository and is not affiliated with, endorsed by, or officially supported by the DeSmuME Project.
