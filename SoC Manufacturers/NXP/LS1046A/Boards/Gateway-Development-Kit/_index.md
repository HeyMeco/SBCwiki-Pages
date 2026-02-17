---
weight: 1
title: Gateway Development Kit
categories:
- board
tags:
- LS1046A
- Layerscape
boards:
- Gateway-Development-Kit
board-vendor:
- Mono
summary: High-performance open-source router development kit powered by NXP Layerscape LS1046A quad-core Cortex-A72 (1.6GHz), 8GB ECC RAM, 2× 10 Gigabit SFP+ ports, 3× Gigabit Ethernet, dual M.2 WiFi slots, 32GB eMMC, OpenWRT pre-installed.
images:
- /images/gateway-mono-01.png
---

# Gateway Development Kit

{{< gallery match="images/*" sortOrder="asc" rowHeight="200" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=false previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware Specifications

{{% details title="Specs" open=true %}}

| **SoC** | **NXP Layerscape LS1046A**                                                                                            |
|---------|-------------------------------------------------------------------------------------------------------------------------------------------|
| **CPU** | 4× ARM Cortex-A72 @ 1.6GHz |
| **RAM** | 8GB DDR4 @ 2100 MT/s with ECC support |

---
### Interfaces

| **I/O**      | Description                                                                                                                                                                                                                                                             |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Storage** | 32GB eMMC (Operating System) <br> 64MB NOR Flash (Bootloader) |
| **Ethernet** | 2× 10 Gigabit SFP+ ports <br> 3× Gigabit Ethernet RJ-45 ports |
| **Wireless** | 2× M.2 Key-E slots: <br> • 1× for WiFi 6 2x2 MU-MIMO <br> • 1× for tri-radio card (WiFi 5 + Bluetooth + Thread) |
| **USB** | 1× USB-C 3.0 port <br> 1× USB-C console/UART port (debugging) |
| **Debugging** | JTAG connector <br> 100+ test points throughout the PCB <br> UART USB-C port <br> Status RGB LED |
| **Cooling** | Active cooling with 2× 4-pin PWM 5V fan headers <br> Heatsink included |
| **Sensors** | 8× power sensors for real-time monitoring <br> 2× temperature sensors |
| **Power** | USB-C PD 3.0 (65W charger included) |
| **Enclosure** | Polycarbonate enclosure with easy access for development |
| **Throughput** | Up to 26 Gbps line-rate for VLANs, PPPoE, and NAT |

{{% /details %}}

{{< list-board-available-os >}}

## Key Features

- **High-Performance Networking**: Up to 26 Gbps line-rate throughput for enterprise networking
- **10 Gigabit Capable**: Dual SFP+ ports for fiber connectivity
- **Open Source**: Built from the ground up with open-source software and transparency
- **Developer-Friendly**: 100+ test points, JTAG, and console access for full control
- **Expandable WiFi**: Dual M.2 slots support WiFi 6 and tri-radio configurations
- **Precision Monitoring**: Real-time power and temperature monitoring throughout the system
- **Active Cooling**: Professional-grade fan and heatsink for sustained performance
- **ECC Memory**: Enterprise-grade 8GB DDR4 with error correction
- **Long-Term Availability**: 10-15 year support commitment

## Product Information

### Development Kit vs Final Product

The Gateway development kit represents the unoptimized version used by the internal development team. It features the highest quality components and manufacturers without any cost optimizations. Two final variants are planned:

- **Founders Edition**: CNC-milled aluminum enclosure
- **Rackmount Edition**: Sheet metal enclosure

All development kit buyers will have the option to purchase a CNC-milled aluminum enclosure to upgrade from the polycarbonate case.

### Operating System Support

- **Pre-installed**: OpenWRT (tested and verified)
- **Tested**: Various Linux distributions, VyOS, VPP + DPDK
- **Compatible**: Any ARM64 software that compiles for the architecture

## Documentation

- [Gateway Product Page](https://mono.si/)

## Where to Buy

- [Mono Official Store](https://mono.si/) - $600 (development kit)
