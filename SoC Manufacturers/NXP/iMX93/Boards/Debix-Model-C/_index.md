---
weight: 1
title: Debix Model C
categories:
- board
tags:
- iMX93
boards:
- Debix-Model-C
board-vendor:
- Polyhex
summary: Low-power industrial SBC powered by NXP i.MX 93 with dual-core Cortex-A55 (1.7GHz), 0.5 TOPS NPU, maximum 1W power consumption, dual Gigabit Ethernet with TSN, -20°C to 70°C operating temperature, and 10-15 year long-term availability.
images:
- /images/debix-model-c-01.png
- /images/debix-model-c-02.png
---

# Debix Model C

{{< gallery match="images/*" sortOrder="asc" rowHeight="200" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=false previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware Specifications

{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 93 (i.MX9352)**                                                                                            |
|---------|-------------------------------------------------------------------------------------------------------------------------------------------|
| **CPU** | 2× ARM Cortex-A55 @ 1.7GHz <br> 1× ARM Cortex-M33 @ 250MHz |
| **RAM** | 1GB LPDDR4X (2GB optional) |
| **NPU** | 0.5 TOPS ARM Ethos-U65 microNPU |
| **GPU** | 2D GPU |

---
### Interfaces

| **I/O**      | Description                                                                                                                                                                                                                                                             |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Storage** | MicroSD card slot <br> Onboard 8MB NOR Flash <br> Optional onboard eMMC: 8GB/16GB/32GB/64GB/128GB/256GB |
| **Ethernet** | 2× Gigabit Ethernet <br> • 1× with TSN support and optional PoE <br> • 1× Gigabit (PoE not supported) |
| **Wireless** | WiFi 5 (2.4GHz & 5GHz) IEEE 802.11a/b/g/n <br> Bluetooth 5.2 <br> External SMA antenna connector (IPEX-1) |
| **USB** | 2× USB 2.0 Host <br> 1× USB 2.0 OTG Type-C |
| **Video** | 1× MIPI DSI 1080p60 (4-lane) <br> 1× LVDS 720p60 (single channel 8-bit) |
| **Camera** | 1× MIPI CSI 1080p60 (2-lane) |
| **Audio** | 3.5mm headphone/mic combo port |
| **Expansion** | 40-pin double-row GPIO header: <br> • 1× I2C, 1× UART (system debug) <br> • 2× USB 2.0 Host <br> • 4× 12-bit ADC input <br> • 6× GPIO (configurable as PWM, UART, SPI, I2C, CAN) <br> • 5V power in/out, 1.8V/3.3V @ 300mA out <br> • System reset, ON/OFF |
| **Other** | 1× 3-bit DIP switch |
| **Power** | DC 5V/2A via USB Type-C <br> **Maximum 1W power consumption** |
| **Security** | EdgeLock® Secure Enclave |
| **Operating Temp** | -20°C to 70°C (standard) <br> -40°C to 85°C (optional) |
| **Dimensions** | 85.0mm × 56.0mm (±0.5mm) |
| **Weight** | 43g net (±0.5g) |

{{% /details %}}

{{< list-board-available-os >}}

## Key Features

- **Ultra-Low Power**: Maximum 1W power consumption at full load, ideal for power-conscious designs
- **Industrial Grade**: Reliable operation from -20°C to 70°C (or -40°C to 85°C) with 10-15 year long-term availability
- **AI Acceleration**: Dedicated 0.5 TOPS NPU for light edge AI applications
- **Time-Sensitive Networking**: TSN-capable Gigabit Ethernet for industrial IT/OT communication
- **Cost-Effective**: Designed for cost-sensitive industrial applications
- **Secure Boot**: EdgeLock® Secure Enclave for enhanced security
- **Flexible Configuration**: Configurable GPIO header for various industrial interfaces

## Use Cases

The Debix Model C is optimized for:
- Power-constrained embedded systems
- Industrial IoT gateways
- Light AI edge processing
- Industrial automation and control
- Smart building applications
- Battery-powered industrial devices

## Documentation

- [Debix Model C Product Page](https://debix.io/product/debix-model-c/)
- [Product Brief](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/Datasheet-ModelC/DEBIX%20Model%20C%20Product%20Brief%20V1.1.pdf)
- [User Manual](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/Datasheet-ModelC/DEBIX%20Model%20C%20User%20Manual%20V1.2.pdf)
- [Schematics](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/Datasheet-ModelC/DEBIX_Model_C_Schematics_V1.1.pdf)
- [3D Model (.stp)](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/Datasheet-ModelC/DEBIX_Model_C_3D.stp)
- [Mechanical Drawing](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/Datasheet-ModelC/DEBIX_Model_C_Mechanical_Drawing_V1.1.pdf)

## Certifications

CE-EMC, C-Tick, FCC, PSE, RoHS, UKCA

## Where to Buy

- [Debix Official Store](https://debix.io/product/debix-model-c/) - $61.99-$87.27
- Configuration-based pricing with options for temperature range, memory, storage, and operating system
