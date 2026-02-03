---
weight: 5
title: Rockchip RK3528
#bookCollapseSection: true
soc-series:
- RK35XX
soc:
- RK3528
tags: 
- SOC-RK
summary: Rockchip RK3528 quad-core ARM processor for Smart IPTV/OTT/DBS and 4K multimedia - Cortex-A53, Mali-450 GPU, 4K decode, HDMI 2.0.
---
# Rockchip RK3528

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **Rockchip RK3528**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Quad-core ARM Cortex-A53 with Neon and FPU, shared L2 Cache            |
| **RAM** | 32-bit DDR3(L)/LPDDR3/DDR4/LPDDR4/LPDDR4X<br>DDR3-2133/DDR3L-2133/LPDDR3-2133/DDR4-2400/LPDDR4(X)-2400, 4GB addressing                                                                                     |
| **GPU** | ARM Mali-450 GPU<br>OpenGL® ES 1.1/2.0, OpenVG 1.1               |
| **VPU** | **Decoder:** H.264/AVC, H.265/HEVC, AVS2 up to 4Kx2K@60fps<br>MPEG-1/2/4, VC-1, AVS/AVS+, H.263<br>**Encoder:** H.264 up to 1080p@60fps, H.265 up to 1080p@60fps, JPEG encoder |
| **Display** | HDMI 2.0b transmitter (4Kx2K@60fps, HDR, CEC, HDCP 2.2)<br>CVBS (720x576@60Hz)                                                                           |
| **Security** | ARM TrustZone, crypto, RNG, firewall                                                                           |
| **Storage** | eMMC 5.1 (HS400, CMD Queue), SD/MMC 4.51, FSPI                                                                           |
| **Connectivity** | USB 2.0 Host, USB 2.0 OTG, USB 3.0 DRD (shared with PCIe 2.1)<br>PCIe 2.1 (1L RC), GbE MAC (RGMII/RMII)<br>SDIO 3.0, 8× UART, 8× I2C, 2× SPI                                                                           |
| **Package** | WBBGA401L (13.3×13.5 mm, 0.65/0.6 mm ball pitch)                                                                           |

{{% /details %}}

---

## Linux Support
{{% columns %}}
- ### Vendor BSP
  - BSP kernel versions

- ### Mainline kernel
  - [ ] Fully supported
  - [x] Works but not all features are implemented.

{{% /columns %}}

---

## Documentation
- [RK3528 Datasheet (FriendlyElec wiki)](https://wiki.friendlyelec.com/wiki/images/7/70/Rockchip_RK3528_Datasheet_V1.2-20240410.pdf)
- Technical Reference Manual

---

## Boards with RK3528

List of boards:

{{< taglist tag="RK3528" style="cards" >}}
