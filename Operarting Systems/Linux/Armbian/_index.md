---
weight: 1
title: Armbian
categories:
- os
#Supported Boards:
boards:
- RPI-5
- Radxa-Rock-5B
---
![Armbian Logo](Armbian-Logo.png?h=150)

# Armbian

[Official Website](https://armbian.com)

## Description

Armbian is a base operating system platform for single board computers (SBCs) that other projects can trust to build upon.

- Lightweight **Debian** or **Ubuntu** based Linux distribution specialized for ARM development boards
- Each system is compiled, assembled and optimized by Armbian Build Tools
- It has powerful build and software development tools to make custom builds
- A vibrant community

### What is the difference between Armbian and Debian/Ubuntu?
- Debian or Ubuntu officially do not support most of those boards/boxes. Armbian does.
- Armbian userspace has many small but vital performance or security adjustments
- Armbian fancy some kernel development and a lot of its maintaining. Debian relies on upstream sources for ARM hardware which can be years behind and/or lack of many functions
- Armbian userspace is lean, clean but 100% Debian/Ubuntu compatible
- Many stock Debian bugs are fixed on the way, “better than original :)”
- The Armbian build system is a central part of this whole ecosystem. You can DIY. Debian is much harder.
- Dedicated support forums per boards/boxes
- Plug’n’Play vs. complicated install scenarios on stock Debian
- unified development scenarios and user experience vs. mess of different setup instructions scattered all around


## Supported Boards

{{< list-os-boards >}}