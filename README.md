# reen

Custom WSL Distribution based on Oracle Linux 8

## About 
Reen is a customized WSL Distribution (based on Oracle Linux 8) for working with MS Azure. This Distribution is produced by my desire to have a WSL Distribution at hand that meet my needs during my work with MS Azure.

There are no plans to submit this Distribution to the Windows Store as this project is currently only driven by my own requirements and I dont see a lot of people finding use for this. If you do however want to try it I welcome you to use it.

I plan to migrate this Distribution to Rocky Linux as soon as the first stable releases appear.

## Installation instruction

### 1. Download

Download the latest release via GitHub releases. You can find all releases her: https://github.com/rooftop90/reen-rootfs/releases  

### 2. Import Distribution
Import the release into your WSL with the following command:
```
wsl --import Reen ./reen release.tar.gz
```

### 3. (Optional) Configure Reen Icon
Update the Reen Terminal configuration stanza to include the graphic assets in [Windows Terminal](https://github.com/microsoft/terminal) settings.json (example):

```
{
    "guid": "{keep the GUID already created}",
    "hidden": false,
    "name": "Reen",
    "source": "Windows.Terminal.Wsl",
    "commandline": "wsl.exe -d reen",
	"icon": "C:\\your\\path\\reen-icon.ico",
}
```

## Reen root-fs builds
The Reen rootfs build are publish through GitHub releases. The repository can be found here: https://github.com/rooftop90/reen-rootfs