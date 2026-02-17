---
weight: 6
title: NXP i.MX 8X
#bookCollapseSection: true
soc-series:
- iMX8X
soc:
- iMX8X
tags: 
- SOC-NXP
- IMX-8
- iMX8X
summary: NXP i.MX 8X ARM processor - Quad-core Cortex-A35 + Cortex-M4, 3D graphics, 4K H.265 video decode, error correcting code on DDR, advanced graphics and efficient performance.
---
# NXP i.MX 8X

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 8X**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Quad-core: <br> 4× ARM Cortex-A35 <br> 1× ARM Cortex-M4            |
| **RAM** | LPDDR4, DDR3L with ECC support                                                                                     |
| **GPU** | 3D GPU, OpenGL ES 3.1, OpenCL 1.2 EP               |
| **VPU** | 4K H.265 video decode <br> 1080p60 H.264/VP8 decode <br> 1080p30 H.264 encode |
| **DSP** | Tensilica HiFi 4 DSP for audio processing                                                                           |
| **Display** | Parallel display, 2× LVDS/MIPI-DSI combo |
| **Camera** | MIPI-CSI (4-lane), Parallel camera interface |
| **Storage** | eMMC 5.1, SD 3.0, Quad SPI |
| **Ethernet** | 2× Gigabit Ethernet |
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
- [NXP i.MX 8X Product Page](https://www.nxp.com/products/i.MX8X)
- [i.MX 8X Family Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX8XIEC.pdf)

---

## Boards with i.MX 8X

List of boards:

{{< taglist tag="iMX8X" style="cards" >}}
