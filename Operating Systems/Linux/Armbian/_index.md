---
weight: 1
title: Armbian
icon: Armbian-Logo.png
summary: Lightweight Debian/Ubuntu-based Linux distribution specialized for ARM development boards
categories:
- os
#Supported Boards:
boards:
- BananaPi-R4
- FriendlyElec-NanoPi-R5S
- Libre-AML-A311D-CC
- Libre-AML-S805X-AC
- Libre-AML-S905X-CC
- Libre-ROC-RK3328-CC
- Libre-ROC-RK3399-PC
- Libre-AML-S905D3-CC
- Libre-AML-S905X-CC-V2
- Libre-ALL-H3-CC
- NVIDIA-Jetson-Nano-DevKit
- OrangePi-5
- Radxa-Cubie-A5E
- Dragon-Q6A
- Dragon-Q8B
- Radxa-NIO-12L
- Radxa-Rock-2A
- Radxa-Rock-2F
- Radxa-Rock-3A
- Radxa-Rock-3C
- Radxa-Rock-4D
- Radxa-Rock-5-ITX
- Radxa-Rock-5A
- Radxa-Rock-5B
- Radxa-Rock-5B+
- Radxa-Rock-5C
- Radxa-Rock-5T
- Radxa-ZERO
- Radxa-ZERO-2-Pro
- Radxa-ZERO-3E
- Radxa-ZERO-3W
- RPI-5
- RPI-500
- RPI-500-Plus
- RPI-Zero-2W
- TI-SK-AM68
- TI-SK-AM69
- Orion-O6
- Orion-O6N
- OrangePi-6-Plus
- Minisforum-MS-R1
- MetaComputing-AI-PC
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

Boards with an Armbian image, from the [Armbian board pages](https://www.armbian.com/boards/).

| Board | Armbian |
|---|---|
| [BananaPi R4](/docs/soc-manufacturers/mediatek/filogic-880/boards/bananapi-r4/) | [`bananapir4`](https://www.armbian.com/boards/bananapir4) |
| [FriendlyElec NanoPi R5S](/docs/soc-manufacturers/rockchip/rk3568/boards/friendlyelec-nanopi-r5s/) | [`nanopi-r5s`](https://www.armbian.com/boards/nanopi-r5s) |
| [Libre Computer Alta (AML-A311D-CC)](/docs/soc-manufacturers/amlogic/a311d/boards/libre-alta/) | [`aml-a311d-cc`](https://www.armbian.com/boards/aml-a311d-cc) |
| [Libre Computer La Frite (AML-S805X-AC)](/docs/soc-manufacturers/amlogic/s805x/boards/libre-la-frite/) | [`lafrite`](https://www.armbian.com/boards/lafrite) |
| [Libre Computer Le Potato (AML-S905X-CC)](/docs/soc-manufacturers/amlogic/s905x/boards/libre-le-potato/) | [`lepotato`](https://www.armbian.com/boards/lepotato) |
| [Libre Computer Renegade (ROC-RK3328-CC)](/docs/soc-manufacturers/rockchip/rk3328/boards/libre-renegade/) | [`renegade`](https://www.armbian.com/boards/renegade) |
| [Libre Computer Renegade Elite (ROC-RK3399-PC)](/docs/soc-manufacturers/rockchip/rk3399/boards/libre-renegade-elite/) | [`roc-rk3399-pc`](https://www.armbian.com/boards/roc-rk3399-pc) |
| [Libre Computer Solitude (AML-S905D3-CC)](/docs/soc-manufacturers/amlogic/s905d3/boards/libre-solitude/) | [`aml-s905d3-cc`](https://www.armbian.com/boards/aml-s905d3-cc) |
| [Libre Computer Sweet Potato (AML-S905X-CC-V2)](/docs/soc-manufacturers/amlogic/s905x/boards/libre-sweet-potato/) | [`sweet-potato`](https://www.armbian.com/boards/sweet-potato) |
| [Libre Computer Tritium (ALL-H3-CC)](/docs/soc-manufacturers/allwinner/h3-h5/boards/libre-tritium/) | [`tritium-h5`](https://www.armbian.com/boards/tritium-h5) |
| [MetaComputing ARM AI PC](/docs/soc-manufacturers/cix/cd8180-p1/boards/metacomputing-ai-pc/) | [`cix-acpi`](https://www.armbian.com/boards/cix-acpi) |
| [Minisforum MS-R1](/docs/soc-manufacturers/cix/cd8180-p1/boards/minisforum-ms-r1/) | [`cix-acpi`](https://www.armbian.com/boards/cix-acpi) |
| [NVIDIA Jetson Nano Developer Kit](/docs/soc-manufacturers/nvidia/tegra-x1/boards/nvidia-jetson-nano-devkit/) | [`jetson-nano`](https://www.armbian.com/boards/jetson-nano) |
| [Orange Pi 5](/docs/soc-manufacturers/rockchip/rk3588/variants/rk3588s/boards/orangepi-5/) | [`orangepi5`](https://www.armbian.com/boards/orangepi5) |
| [Orange Pi 6 Plus](/docs/soc-manufacturers/cix/cd8180-p1/boards/orangepi-6-plus/) | [`cix-acpi`](https://www.armbian.com/boards/cix-acpi) |
| [Radxa Cubie A5E](/docs/soc-manufacturers/allwinner/a527/boards/radxa-cubie-a5e/) | [`radxa-cubie-a5e`](https://www.armbian.com/boards/radxa-cubie-a5e) |
| [Radxa Dragon Q6A](/docs/soc-manufacturers/qualcomm/dragonwing-6490/boards/radxa-dragon-q6a/) | [`radxa-dragon-q6a`](https://www.armbian.com/boards/radxa-dragon-q6a) |
| [Radxa Dragon Q8B](/docs/soc-manufacturers/qualcomm/sc8280xp/boards/radxa-dragon-q8b/) | [`radxa-dragon-q8b`](https://www.armbian.com/boards/radxa-dragon-q8b) |
| [Radxa NIO 12L](/docs/soc-manufacturers/mediatek/genio-1200/boards/radxa-nio-12l/) | [`radxa-nio-12l`](https://www.armbian.com/boards/radxa-nio-12l) |
| [Radxa Orion O6](/docs/soc-manufacturers/cix/cd8180-p1/boards/radxa-orion-o6/) | [`cix-acpi`](https://www.armbian.com/boards/cix-acpi) |
| [Radxa Orion O6N](/docs/soc-manufacturers/cix/cd8180-p1/boards/radxa-orion-o6n/) | [`cix-acpi`](https://www.armbian.com/boards/cix-acpi) |
| [Radxa Rock 2A](/docs/soc-manufacturers/rockchip/rk3528/boards/radxa-rock-2a/) | [`rock-2a`](https://www.armbian.com/boards/rock-2a) |
| [Radxa Rock 2F](/docs/soc-manufacturers/rockchip/rk3528/boards/radxa-rock-2f/) | [`rock-2f`](https://www.armbian.com/boards/rock-2f) |
| [Radxa Rock 3A](/docs/soc-manufacturers/rockchip/rk3568/boards/radxa-rock-3a/) | [`rock-3a`](https://www.armbian.com/boards/rock-3a) |
| [Radxa Rock 3C](/docs/soc-manufacturers/rockchip/rk3566/boards/radxa-rock-3c/) | [`rock-3c`](https://www.armbian.com/boards/rock-3c) |
| [Radxa Rock 4D](/docs/soc-manufacturers/rockchip/rk3576/boards/radxa-rock-4d/) | [`radxa-rock-4d`](https://www.armbian.com/boards/radxa-rock-4d) |
| [Radxa Rock 5 ITX](/docs/soc-manufacturers/rockchip/rk3588/boards/radxa-rock-5-itx/) | [`rock-5-itx`](https://www.armbian.com/boards/rock-5-itx) |
| [Radxa Rock 5A](/docs/soc-manufacturers/rockchip/rk3588/variants/rk3588s/boards/radxa-rock-5a/) | [`rock-5a`](https://www.armbian.com/boards/rock-5a) |
| [Radxa Rock 5B](/docs/soc-manufacturers/rockchip/rk3588/boards/radxa-rock-5b/) | [`rock-5b`](https://www.armbian.com/boards/rock-5b) |
| [Radxa Rock 5B+](/docs/soc-manufacturers/rockchip/rk3588/boards/radxa-rock-5b+/) | [`rock-5b-plus`](https://www.armbian.com/boards/rock-5b-plus) |
| [Radxa Rock 5C](/docs/soc-manufacturers/rockchip/rk3588/variants/rk3588s/boards/radxa-rock-5c/) | [`rock-5c`](https://www.armbian.com/boards/rock-5c) |
| [Radxa Rock 5T](/docs/soc-manufacturers/rockchip/rk3588/boards/radxa-rock-5t/) | [`rock-5t`](https://www.armbian.com/boards/rock-5t) |
| [Radxa ZERO](/docs/soc-manufacturers/amlogic/s905y2/boards/radxa-zero/) | [`radxa-zero`](https://www.armbian.com/boards/radxa-zero) |
| [Radxa ZERO 2 Pro](/docs/soc-manufacturers/amlogic/a311d/boards/radxa-zero-2-pro/) | [`radxa-zero2`](https://www.armbian.com/boards/radxa-zero2) |
| [Radxa ZERO 3E](/docs/soc-manufacturers/rockchip/rk3566/boards/radxa-zero-3e/) | [`radxa-zero3`](https://www.armbian.com/boards/radxa-zero3) |
| [Radxa ZERO 3W](/docs/soc-manufacturers/rockchip/rk3566/boards/radxa-zero-3w/) | [`radxa-zero3`](https://www.armbian.com/boards/radxa-zero3) |
| [Raspberry Pi 5](/docs/soc-manufacturers/broadcom/bcm2712/boards/rasperrypi-5/) | [`raspberrypi5`](https://www.armbian.com/boards/raspberrypi5) |
| [Raspberry Pi 500](/docs/soc-manufacturers/broadcom/bcm2712/boards/raspberrypi-500/) | [`raspberrypi500`](https://www.armbian.com/boards/raspberrypi500) |
| [Raspberry Pi 500+](/docs/soc-manufacturers/broadcom/bcm2712/boards/raspberrypi-500-plus/) | [`raspberrypi500plus`](https://www.armbian.com/boards/raspberrypi500plus) |
| [Raspberry Pi Zero 2 W](/docs/soc-manufacturers/broadcom/rp3a0/boards/raspberrypi-zero-2w/) | [`raspberrypizero2w`](https://www.armbian.com/boards/raspberrypizero2w) |
| [TI SK-AM68](/docs/soc-manufacturers/texas-instruments/am68a/boards/ti-sk-am68/) | [`sk-am68`](https://www.armbian.com/boards/sk-am68) |
| [TI SK-AM69](/docs/soc-manufacturers/texas-instruments/am69a/boards/ti-sk-am69/) | [`sk-am69`](https://www.armbian.com/boards/sk-am69) |


Further images are available on the [download page](https://www.armbian.com/download/)