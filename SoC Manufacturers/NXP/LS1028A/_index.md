---
weight: 15
title: NXP Layerscape LS1028A
#bookCollapseSection: true
soc-series:
- Layerscape
soc:
- LS1028A
tags: 
- SOC-NXP
- Layerscape
- LS1028A
summary: NXP Layerscape LS1028A networking processor - Dual Cortex-A72 cores (up to 1.3GHz), 2× PCIe Gen 3.0, 5× 2.5 Gigabit Ethernet with TSN, eDP/DP display support, industrial and edge computing applications.
---
# NXP Layerscape LS1028A

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP Layerscape LS1028A**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Dual-core: <br> 2× ARM Cortex-A72 (up to 1.3GHz)            |
| **RAM** | DDR3L, DDR4                                                                                     |
| **Ethernet** | 5× 2.5 Gigabit Ethernet + 1× Gigabit Ethernet with TSN support |
| **Display** | LCD controller with eDP/DP output |
| **PCIe** | 2× PCIe Gen 3.0 |
| **SerDes** | 4-10 GHz SerDes lanes |
| **Storage** | SD, SPI, I²C |
| **SATA** | 1× SATA 3.0 |
| **Security** | SEC security engine, 5 Gbit/s |
| **USB** | USB 2.0/3.0 |

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented.

See [Layerscape device trees](https://github.com/torvalds/linux/tree/master/arch/arm64/boot/dts/freescale) in mainline Linux kernel

### Vendor BSP
- NXP provides [linux-qoriq kernel](https://github.com/nxp-qoriq/linux) and [Layerscape SDK](https://www.nxp.com/design/design-center/software/embedded-software/linux-software-and-development-tools/layerscape-linux-distribution-poc:LAYERSCAPE-SDK) with Yocto-based Linux distribution

---

## Documentation
- [NXP LS1028A Product Page](https://www.nxp.com/products/LS1028A)
- [Layerscape Software Development Kit](https://www.nxp.com/design/design-center/software/embedded-software/linux-software-and-development-tools/layerscape-linux-distribution-poc:LAYERSCAPE-SDK)

---

## Boards with LS1028A

List of boards:

{{< taglist tag="LS1028A" style="cards" >}}
