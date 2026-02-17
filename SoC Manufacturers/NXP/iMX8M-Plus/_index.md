---
weight: 5
title: NXP i.MX 8M Plus
#bookCollapseSection: true
soc-series:
- iMX8M
soc:
- iMX8M-Plus
tags: 
- SOC-NXP
- IMX-8
- iMX8M-Plus
summary: NXP i.MX 8M Plus ARM processor - Quad-core Cortex-A53 (up to 1.8GHz) + Cortex-M7 (800MHz), GC7000UL GPU, 2.3 TOPS NPU for machine learning, dual camera ISP, 14nm FinFET process.
---
# NXP i.MX 8M Plus

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 8M Plus**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **Process** | 14nm LPC FinFET |
| **CPU** | Quad-core: <br> 4× ARM Cortex-A53 (up to 1.8GHz commercial, 1.6GHz industrial) <br> 1× ARM Cortex-M7 (800MHz)            |
| **RAM** | LPDDR4                                                                                     |
| **GPU** | Vivante GC7000UL, 1 GPixel/s, OpenGL ES 3.1, Vulkan, OpenCL 1.2 FP               |
| **NPU** | 2.3 TOPS Neural Processing Unit for ML acceleration                                                                           |
| **VPU** | 1080p60 H.265/H.264/VP9/VP8 decode <br> 1080p60 H.265/H.264 encode |
| **ISP** | Dual Camera ISP, 375 MPixels/s |
| **Display** | MIPI-DSI (4-lane), HDMI 2.0, LVDS |
| **Camera** | 2× MIPI-CSI (4-lane each) |
| **Storage** | eMMC 5.1, SD 3.0, Quad SPI |
| **Ethernet** | 2× Gigabit Ethernet (1× with TSN) |
| **PCIe** | PCIe Gen 3.0 |

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented.

See [i.MX device trees](https://github.com/torvalds/linux/tree/master/arch/arm64/boot/dts/freescale) in mainline Linux kernel

### Vendor BSP
- NXP provides [linux-imx kernel](https://github.com/nxp-imx/linux-imx) and [Yocto-based BSP](https://www.nxp.com/design/design-center/software/embedded-software/i-mx-software/embedded-linux-for-i-mx-applications-processors:IMXLINUX) with Long Term Support

---

## Documentation
- [NXP i.MX 8M Plus Product Page](https://www.nxp.com/products/i.MX8MPLUS)
- [i.MX 8M Plus Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX8MPIEC.pdf)

---

## Boards with i.MX 8M Plus

List of boards:

{{< taglist tag="iMX8M-Plus" style="cards" >}}
