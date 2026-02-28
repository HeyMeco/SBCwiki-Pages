---
weight: 3
title: OpenMediaVault
icon: OMV-Logo.png
iconBg: "#8ed1fc"
summary: Network-attached storage (NAS) solution based on Debian Linux for home and small office use
categories:
- os
#Supported Boards:
#All boards with Armbian or Debian
---
![OpenMediaVault Logo](OMV-Logo.png?w=400&bc=8ed1fc)

# OpenMediaVault

[Official Website](https://www.openmediavault.org/)

## Description

Openmediavault is the next generation network attached storage (NAS) solution based on Debian Linux. It contains services like SSH, (S)FTP, SMB/CIFS, RSync and many more ready to use. Thanks to the modular design of the framework it can be enhanced via plugins. Openmediavault is primarily designed to be used in small offices or home offices, but is not limited to those scenarios. It is a simple and easy to use out-of-the-box solution that will allow everyone to install and administrate a Network Attached Storage without deeper knowledge.

## Features
{{% columns %}}
- - Running out-of-the-box
  - Debian Linux OS
  - Web based administration
  - Easy system updates via Debian package management
  - Volume management
  - S.M.A.R.T.

- - Link aggregation
  - Wake On Lan
  - IPv6 support
  - Email notifications
  - File sharing
  - Snapshot support of shared folders
  - Extendible via plugins
{{% /columns %}}

## Versions

| OMV Version | Codename | Debian Base | Status |
|-------------|----------|-------------|--------|
| 5.x | Usul | Debian 10 (Buster) | EOL (Jun 2022) |
| 6.x | Shaitan | Debian 11 (Bullseye) | EOL (Jul 2024) |
| 7.x | Sandworm | Debian 12 (Bookworm) | Stable |
| 8.x | Synchrony | Debian 13 (Trixie) | Current (Dec 2025) |

## Supported Boards

**All boards that have minimal Debian 12 (OMV7) or Debian 13 (OMV8) available for example through Armbian with [the install script](https://github.com/OpenMediaVault-Plugin-Developers/installScript)**

> [!NOTE]
> OMV 8.x only supports AMD64 and ARM64 architectures.