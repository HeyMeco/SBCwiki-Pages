---
weight: 2
title: NXP i.MX 8M
#bookCollapseSection: true
soc-series:
- iMX8M
soc:
- iMX8M
tags: 
- SOC-NXP
- IMX-8
- iMX8M
summary: NXP i.MX 8M ARM processor - Quad-core Cortex-A53 (up to 1.5GHz) + Cortex-M4, GC7000Lite GPU, 4Kp60 H.265/VP9 video decode, advanced audio and voice processing, 14nm FinFET process.
---
# NXP i.MX 8M

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 8M**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **Process** | 14nm LPC FinFET |
| **CPU** | Quad-core: <br> 4× ARM Cortex-A53 (up to 1.5GHz) <br> 1× ARM Cortex-M4            |
| **RAM** | LPDDR4, DDR3L                                                                                     |
| **GPU** | Vivante GC7000Lite, OpenGL ES 3.1, Vulkan               |
| **VPU** | 4Kp60 H.265/VP9 video decode with HDR <br> 4Kp30 H.264/VP8 decode <br> 1080p30 H.264 encode |
| **Display** | MIPI-DSI (4-lane), HDMI 2.0a |
| **Camera** | 2× MIPI-CSI (4-lane each) |
| **Storage** | eMMC 5.1, SD 3.0, Quad SPI |
| **Ethernet** | Gigabit Ethernet |

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
- [NXP i.MX 8M Product Page](https://www.nxp.com/products/i.MX8M)
- [i.MX 8M Family Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX8MDQLQCEC.pdf)

---

## Boards with i.MX 8M

List of boards:

{{< taglist tag="iMX8M" style="cards" >}}
