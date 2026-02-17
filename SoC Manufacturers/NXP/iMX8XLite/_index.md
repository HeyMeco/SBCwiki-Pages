---
weight: 7
title: NXP i.MX 8XLite
#bookCollapseSection: true
soc-series:
- iMX8X
soc:
- iMX8XLite
tags: 
- SOC-NXP
- IMX-8
- iMX8XLite
summary: NXP i.MX 8XLite ARM processor - Dual-core Cortex-A35 + Cortex-M4, secure telematics and connected industrial control, 2× Gigabit Ethernet with TSN and AVB support.
---
# NXP i.MX 8XLite

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 8XLite**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Dual-core: <br> 2× ARM Cortex-A35 <br> 1× ARM Cortex-M4            |
| **RAM** | LPDDR4, DDR3L                                                                                     |
| **Display** | Parallel display interface |
| **Storage** | eMMC 5.1, SD 3.0, SPI |
| **Ethernet** | 2× Gigabit Ethernet with TSN and AVB support |
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
- [NXP i.MX 8XLite Product Page](https://www.nxp.com/products/iMX8XLite)

---

## Boards with i.MX 8XLite

List of boards:

{{< taglist tag="iMX8XLite" style="cards" >}}
