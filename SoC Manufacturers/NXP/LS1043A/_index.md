---
weight: 16
title: NXP Layerscape LS1043A
#bookCollapseSection: true
soc-series:
- Layerscape
soc:
- LS1043A
tags: 
- SOC-NXP
- Layerscape
- LS1043A
summary: NXP Layerscape LS1043A networking processor - Quad Cortex-A53 cores (up to 1.6GHz), 3× PCIe Gen 2.0, 1× 10 Gigabit Ethernet + up to 5× Gigabit Ethernet, SEC security engine with 5 Gbit/s throughput.
---
# NXP Layerscape LS1043A

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP Layerscape LS1043A**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Quad-core: <br> 4× ARM Cortex-A53 (up to 1.6GHz)            |
| **RAM** | DDR3L, DDR4                                                                                     |
| **Ethernet** | 1× 10 Gigabit Ethernet + up to 5× Gigabit Ethernet |
| **PCIe** | 3× PCIe Gen 2.0 |
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
- [NXP LS1043A Product Page](https://www.nxp.com/products/LS1043A)
- [Layerscape Software Development Kit](https://www.nxp.com/design/design-center/software/embedded-software/linux-software-and-development-tools/layerscape-linux-distribution-poc:LAYERSCAPE-SDK)

---

## Boards with LS1043A

List of boards:

{{< taglist tag="LS1043A" style="cards" >}}
