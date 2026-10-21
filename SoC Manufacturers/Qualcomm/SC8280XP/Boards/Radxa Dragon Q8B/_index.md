---
weight: 1
title: Radxa Dragon Q8B
categories:
- board
tags: 
- SC8280XP
boards:
- Dragon-Q8B
board-vendor:
- Radxa
summary: "Radxa Dragon Q8B single-board computer - Snapdragon 8cx Gen 3, up to 32GB LPDDR4X, Adreno 690 GPU, dual 2.5GbE, triple 4K120 display output."
images:
- images/1-q8b_top.webp
- images/2-q8b_bottom.webp
---

# Radxa Dragon Q8B

## Board Pictures
{{< gallery match="images/*" sortOrder="asc" rowHeight="150" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=true previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware
{{% details title="Specs" open=true %}}

| **SoC** | **Qualcomm Snapdragon 8cx Gen 3 (SC8280XP)**                                                                                                                      |
|---------|-------------------------------------------------------------------------------------------------------------------------------------------|
| **CPU** | 4x Arm Cortex-X1 @ 3.0GHz<br>4x Arm Cortex-A78 @ 2.4GHz                                                             |
| **RAM** | LPDDR4X up to 4266 MT/s, 128-bit<br>- Up to 32GB                                                                                |
| **GPU** | Qualcomm Adreno 690<br>- OpenGL ES 3.2<br>- Vulkan 1.3<br>- OpenCL 2.0<br>- DirectX<br>- DirectML                                                 |
| **AI**  | Qualcomm Hexagon processor and Sensing Hub<br>- Qualcomm AI Engine up to 29+ TOPS                                                 |
| **VPU** | Decode up to 4K120 (H.265 Main 10 / H.265 Main / H.264 High / VP9 Profile 2)<br>Encode up to 4K60 (H.265 Main 10 / H.265 Main / H.264 High)                          |

---
### Interfaces

| **I/O**      | Description                                                                                                                                                                                                                                                             |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Wireless** | 1x M.2 E Key 2230 for a Wi-Fi 6E / Bluetooth 5.3 module<br>V1.3 and later can use a Wi-Fi 7 module                                                                                                                                                                                                                      |
| **Ethernet** | 2x 2.5GbE RJ45 (QPS615 PCIe bridge, AVB/TSN)                                                                                                                                                                                                        |
| **USB**      | 2x USB 3.2 Gen 2 Type-C (DisplayPort 1.4 Alt Mode)<br>2x USB 3.2 Gen 2 Type-A<br>2x USB 2.0 Type-A<br>1x USB Type-C power input                                                                                                                                                                                                                 |
| **Video**    | 1x HDMI 2.1, up to 4K120<br>2x USB Type-C DisplayPort 1.4 Alt Mode, up to 4K120                                                                                                                                                                                                                     |
| **Camera**   | 1x 50-pin board-to-board connector (PCIe / MIPI CSI / I2C)                                                                                                                                                                                                                                |
| **Audio**    | 3.5 mm headphone jack<br>Microphone connector                                                                                                   |
| **Storage**  | Boot: onboard SPI NOR flash<br>1x UFS 3.1 module (Gear 4 x2)<br>1x microSD<br>1x M.2 M Key 2280 (PCIe 3.0 x4)<br>1x M.2 M Key 2280 (PCIe 3.0 x2)                                                                                                                                                            |
| **Power**    | USB Type-C, 20V<br>12–20V power header with external power-button pin                                                                                                                                                            |
| **GPIO**     | 40-pin header (UART, I2C, SPI, GPIO)                                                                                                                                                                                                                              |
| **Other**    | 1x FPC (PCIe 3.0 x1)<br>RTC battery connector<br>Fan connector<br>Power button, EDL button<br>100 mm × 75 mm                                                                                                                                                                                                              |

{{% /details %}}

## Available OS images
- Radxa OS
- Windows on Arm
- Ubuntu
- [Armbian](https://www.armbian.com/radxa-dragon-q8b/)
- Arch Linux
- NixOS
- Debian

## Documentation / Links

- [Vendor Docs](https://docs.radxa.com/en/dragon/q8b)
- [Product brief](https://dl.radxa.com/dragon/q8b/docs/radxa_dragon_q8b_product_brief_en.pdf)

## Benchmarks

- Geekbench 6.7.1 Preview, Armbian 26.08 (kernel 7.0.11-midstream-sc8280xp):<br> Single Core **1663**, Multi Core **6852**

## Guides

- [Radxa Dragon Q8B documentation](https://docs.radxa.com/en/dragon/q8b)
