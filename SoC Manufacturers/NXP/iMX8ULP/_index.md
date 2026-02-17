---
weight: 8
title: NXP i.MX 8ULP
#bookCollapseSection: true
soc-series:
- iMX8ULP
soc:
- iMX8ULP
tags: 
- SOC-NXP
- IMX-8
- iMX8ULP
summary: NXP i.MX 8ULP ARM processor - Ultra-low power dual-core Cortex-A35 + dual Cortex-M33, Energy Flex architecture, 2D GPU, MIPI-DSI display, industrial and mobile applications.
---
# NXP i.MX 8ULP

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 8ULP**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Dual-core: <br> 2× ARM Cortex-A35 <br> 2× ARM Cortex-M33            |
| **RAM** | LPDDR4, LPDDR4X                                                                                     |
| **GPU** | 2D GPU, OpenVG 1.1               |
| **Display** | MIPI-DSI (4-lane), 24-bit RGB, EPD (E-Paper Display) |
| **Camera** | MIPI-CSI (2-lane) |
| **Storage** | eMMC 5.1, SD 3.0, Quad SPI |
| **Ethernet** | Gigabit Ethernet |
| **Power** | Energy Flex architecture for ultra-low power consumption |
| **Security** | EdgeLock secure enclave |

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
- [NXP i.MX 8ULP Product Page](https://www.nxp.com/products/i.MX8ULP)
- [i.MX 8ULP Whitepaper](https://www.nxp.com/webapp/Download?colCode=IMX8ULPWP)

---

## Boards with i.MX 8ULP

List of boards:

{{< taglist tag="iMX8ULP" style="cards" >}}
