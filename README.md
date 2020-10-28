# Arch GRIT (Graphical Recovery and Installation Tool) - WIP

A custom, graphical Arch Linux live environment, built with [Archiso](https://wiki.archlinux.org/index.php/Archiso).</br>
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

### Minimal: (for DIYers)
 - Follows the [Official Installation Guide](https://wiki.archlinux.org/index.php/Installation_guide) to the letter.
 - Does **not** proceed beyond the end of the Official Installation Guide, any additional setup must be performed by the user.
 - Only allows for customizing the basic installation parameters (filesystem, kernel, hostname, passwords, etc.)
 - Absolutely no extras included. This is as bare-bones as it gets. A true, basic Arch install.

### Graphical: (for most users)
 - Full graphical installation with your choice of officially supported [Desktop Environment](https://wiki.archlinux.org/index.php/Desktop_environment#Officially_supported) or Window Manager.
 - Some basic Quality of Life configurations done for you:
    - Enable SSD TRIM support if appropriate.
    - Enable the pacman cache cleaner service.
 - Includes some non-optional extras:
    - `base-devel` - Development Tools
    - `firefox`    - Web Browser

### Ultimate: (pure bloat?)
 - AwesomeWM with a complex, almost Desktop Environment-like theme.
 - The same QoL configurations, and non-optional extras, from the Graphical installation.
 - Even more non-optional extras:
    - `discord` - Chat App
    - `firefox` - Web Browser
    - `steam`   - Game Store

## Usage
