---
weight: 1
title: Armbian
icon: Armbian-Logo.png
summary: Lightweight Debian/Ubuntu-based Linux distribution specialized for ARM development boards
categories:
- os
#Supported Boards:
boards:
- RPI-5
- Radxa-Rock-5B
- Dragon-Q6A
---
![Armbian Logo](Armbian-Logo.png?h=150)

# Armbian

[Official Website](https://armbian.com)

[Armbian Imager](https://imager.armbian.com/)

[Github Page for Build TUI](https://github.com/armbian/build)

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

## Installation

### Via Armbian Imager to SD Card

{{% steps %}}
1. ## Select Manufacturer
   Choose from 70+ supported SBC manufacturers or load a custom image.

2. ## Select Board
   Pick your board using real photos and metadata from armbian.com.

3. ## Select Image
   Choose desktop or server, kernel variant, and stable or nightly builds.

4. ## Flash
   Download, decompress, write, and verify automatically.
{{% /steps %}}

### Build your custom image with armbian/build

{{% steps %}}
1. ## Git Clone armbian/build
   `git clone https://github.com/armbian/build.git`

2. ## Run compile.sh
   `./compile.sh`

3. ## Select Your Board, ...
   - Ubuntu or Debian
   - Version
   - Minimal or Desktop 
   
   and customize it to your needs with the available options

4. ## Flash to SD Card
   Simply with Armbian Imager by selecting custom image
{{% /steps %}}

## Supported Boards

{{< list-os-boards >}}

Further images are available on the [download page](https://www.armbian.com/download/)