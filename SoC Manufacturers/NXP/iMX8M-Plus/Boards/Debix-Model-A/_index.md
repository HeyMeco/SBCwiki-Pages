---
weight: 1
title: Debix Model A
categories:
- board
tags:
- iMX8M-Plus
- IMX-8
boards:
- Debix-Model-A
board-vendor:
- Polyhex
summary: Industrial SBC powered by NXP i.MX 8M Plus with quad-core Cortex-A53 (up to 1.8GHz), 2.3 TOPS NPU, dual Gigabit Ethernet with TSN, 4x USB 3.0, -20°C to 70°C operating temperature, and 10-15 year long-term availability.
images:
- /images/debix-model-a-01.png
- /images/debix-model-a-02.png
---

# Debix Model A

{{< gallery match="images/*" sortOrder="asc" rowHeight="200" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=false previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware Specifications

{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 8M Plus (Quad-core or Quad Lite variants)**                                                                                            |
|---------|-------------------------------------------------------------------------------------------------------------------------------------------|
| **CPU** | 4× ARM Cortex-A53 @ 1.6GHz (industrial) / 1.8GHz (commercial) <br> 1× ARM Cortex-M7 @ 800MHz |
| **RAM** | 2GB LPDDR4 (4GB/8GB optional) |
| **NPU** | 2.3 TOPS Neural Processing Unit (Standard version) |
| **GPU** | Vivante GC7000UL 3D GPU <br> Vivante GC520L 2D GPU |
| **VPU** | 1080p60 H.265/H.264 encode/decode |
| **ISP** | Dual camera ISP, 375 MPixels/s |

---
### Interfaces

| **I/O**      | Description                                                                                                                                                                                                                                                             |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Storage** | MicroSD card slot <br> Optional onboard eMMC: 8GB/16GB/32GB/64GB/128GB/256GB |
| **Ethernet** | 2× Gigabit Ethernet <br> • 1× with TSN support and optional PoE <br> • 1× via 12-pin header (without transformer) |
| **Wireless** | WiFi 5 (2.4GHz & 5GHz) <br> Bluetooth 5.0 <br> External SMA antenna connector (IPEX-4) |
| **USB** | 4× USB 3.0 Host <br> 1× USB 2.0 OTG Type-C |
| **Video** | 1× HDMI 2.0a output <br> 1× MIPI DSI (4-lane) <br> 1× LVDS (single & dual channel 8-bit) |
| **Camera** | 1× MIPI CSI (4-lane) |
| **Audio** | 3.5mm headphone/mic combo port <br> SPDIF digital audio |
| **Expansion** | 40-pin double-row GPIO header: <br> • 3× UART, 2× I2C, 2× SPI, 2× CAN <br> • 6× GPIO (configurable as I2S, PWM, SPDIF) <br> • 5V power supply, system reset, ON/OFF |
| **PCIe** | 1× PCIe Gen 3.0 (1-lane) |
| **Power** | DC 5V/3A via USB Type-C |
| **Security** | Integrated EdgeLock® Secure Enclave |
| **Operating Temp** | -20°C to 70°C (Model A) <br> -40°C to 85°C (Model B) |
| **Dimensions** | 85.0mm × 56.0mm (±0.5mm) |
| **Weight** | 46g net / 72g gross (±0.5g) |

{{% /details %}}

{{< list-board-available-os >}}

## Key Features

- **Industrial Grade**: Reliable operation from -20°C to 70°C with 10-15 year long-term availability
- **AI Acceleration**: Dedicated 2.3 TOPS NPU for edge AI applications
- **Time-Sensitive Networking**: TSN-capable Gigabit Ethernet for industrial IT/OT communication
- **Multimedia**: Advanced video encode/decode with 3D/2D graphics acceleration
- **Flexible I/O**: 40-pin header configurable for various industrial interfaces
- **Secure Boot**: EdgeLock® Secure Enclave for enhanced security

## Product Variants

### Standard vs Lite

| Feature | Standard | Lite |
|---------|----------|------|
| NPU | ✓ (2.3 TOPS) | ✗ |
| VPU | ✓ | ✗ |
| ISP | ✓ | ✗ |
| HiFi 4 DSP | ✓ | ✗ |

## Documentation

- [Debix Model A Product Page](https://debix.io/product/debix-model-a/)
- [Debix Model A Hardware Documentation](https://debix.io/hardware/model-a.html)
- [Product Brief](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/Datasheet-ModelA/DEBIX_Model_A_Product_Brief_V2.0.pdf)
- [User Manual](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/DEBIX%20User%20Manual%20V2.4.pdf)
- [Schematics](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/DEBIX_Model_A_Schematics_V1.2.pdf)
- [3D Model (.stp)](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/DEBIX_Model_A_3D.stp)
- [Mechanical Drawing](https://debix-oss.oss-cn-hongkong.aliyuncs.com/debix/DEBIX_Model_A_Mechanical_Drawing_V1.1.pdf)

## Certifications

CE, FCC, UKCA, RCM, MIC (TELEC), KC, RoHS

## Where to Buy

- [Debix Official Store](https://debix.io/product/debix-model-a/) - $133.87-$177.09
- Configuration-based pricing with options for memory, storage, and operating system
