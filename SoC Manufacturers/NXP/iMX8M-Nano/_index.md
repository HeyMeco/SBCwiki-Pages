---
weight: 4
title: NXP i.MX 8M Nano
#bookCollapseSection: true
soc-series:
- iMX8M
soc:
- iMX8M-Nano
tags: 
- SOC-NXP
- IMX-8
- iMX8M-Nano
summary: NXP i.MX 8M Nano ARM processor - Quad-core Cortex-A53 (up to 1.5GHz) + Cortex-M7 (800MHz), optional 3D GPU with OpenGL ES 3.1 and Vulkan, 14nm FinFET process.
---
# NXP i.MX 8M Nano

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 8M Nano**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **Process** | 14nm LPC FinFET |
| **CPU** | Quad-core: <br> 4× ARM Cortex-A53 (up to 1.5GHz) <br> 1× ARM Cortex-M7 (up to 750MHz)            |
| **RAM** | LPDDR4, DDR4, DDR3L                                                                                     |
| **GPU** | Optional 3D GPU, OpenGL ES 3.1, Vulkan               |
| **Display** | MIPI-DSI (4-lane) |
| **Camera** | MIPI-CSI (2-lane) |
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
- [NXP i.MX 8M Nano Product Page](https://www.nxp.com/products/i.MX8MNANO)
- [i.MX 8M Nano Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX8MNEC.pdf)

---

## Boards with i.MX 8M Nano

List of boards:

{{< taglist tag="iMX8M-Nano" style="cards" >}}
