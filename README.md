# Arch GRIT (Graphical Recovery and Installation Tool)

#### A custom, graphical Arch Linux live environment, built with [`archiso`](https://wiki.archlinux.org/index.php/Archiso).</br>
**Features:**
 - Graphical desktop environment, with standard tools such as file and web browser.
 - Modular, customizable Arch Linux installation script with 3 **Installation Types**:
    - Minimal: Installed as per the [Official Installation Guide](https://wiki.archlinux.org/index.php/Installation_guide), no customization, no extras.
    - Graphical: Graphical installation, with various customization options.
    - Ultimate: My personal installation, designed for nerds and power users.
 - Various scripts and software packages to aid with the recovery of any system.
 - No more password-less login as root! Keep unintended users **out** of the installation environment!
<br>

## Installation Types

#### Minimal: (for DIYers)
 - Follows the [Official Installation Guide](https://wiki.archlinux.org/index.php/Installation_guide) to the letter.
 - Does **not** proceed beyond the end of the Official Installation Guide, any additional setup must be performed by the user.
 - Only allows for customizing the basic installation parameters (filesystem, kernel, hostname, passwords, etc.)
 - Absolutely no extras included. This is as bare-bones as it gets. A true, basic Arch install.

#### Graphical: (for most users)
 - Full graphical installation with your choice of officially supported [Desktop Environment](https://wiki.archlinux.org/index.php/Desktop_environment#Officially_supported) or Window Manager.
 - Some basic Quality of Life configurations done for you:
    - Enable SSD TRIM support if appropriate.
    - Enable the pacman cache cleaner service.
 - Includes some non-optional extras:
    - `base-devel` - Development Tools
    - `firefox` - Web Browser

#### Ultimate: (pure bloat?)
 - AwesomeWM with a complex, almost Desktop Environment-like theme.
 - The same QoL configurations, and non-optional extras, from the Graphical installation.
 - Even more non-optional extras:
    - `discord` - Chat App
    - `firefox` - Web Browser
    - `steam` - Game Store
<br>

## Usage
 - Build the ISO image, or download the pre-built image.
 - Write the image to a USB flash drive.
 - Boot the USB flash drive.
 - Log in as `live_user` with the password `archlinux`.
 - Run `arch-grit install` for the installation menu.
<br>

## Build Instructions

Building this project requires a functional Arch Linux system, with [`archiso`](https://www.archlinux.org/packages/extra/any/archiso/) installed.
For those of you whom are **not** running Arch Linux already, there is a signed, pre-built ISO available [here](https://github.com/ryyzer/arch-grit).

#### Building
 - `git clone https://github.com/ryyzer/arch-grit`
 - `cd arch-grit/aur_repo`
 - `./refresh-packages.sh`
 - `cd ..`
 - `mkarchiso -v .`

#### Writing to USB flash drive
**WARNING:** Please be careful with the `dd` command, it is relatively easy to wipe out an entire drive worth of data.
 - `sudo dd bs=4M status=progress oflag=sync if=out/arch-grit.iso of=/dev/sdX`
<br>
---
