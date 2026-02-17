---
weight: 19
title: NXP Layerscape LS2088A
#bookCollapseSection: true
soc-series:
- Layerscape
soc:
- LS2088A
tags: 
- SOC-NXP
- Layerscape
- LS2088A
summary: NXP Layerscape LS2088A networking processor - Octa-core Cortex-A72 (up to 2.1GHz), 4× PCIe Gen 3.0, 8× 10 Gigabit Ethernet + 8× Gigabit Ethernet, 88 Gbit/s L2 switching, DPAA2 acceleration engines.
---
# NXP Layerscape LS2088A

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP Layerscape LS2088A**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Octa-core: <br> 8× ARM Cortex-A72 (up to 2.1GHz)            |
| **RAM** | DDR4                                                                                     |
| **Ethernet** | 8× 10 Gigabit Ethernet (up to 1/2.5/10 Gbit/s) + 8× Gigabit Ethernet (2.5/1 Gbit/s) |
| **L2 Switch** | 88 Gbit/s L2 switching capability |
| **PCIe** | 4× PCIe Gen 3.0 |
| **SerDes** | 16× 10 GHz SerDes lanes |
| **Storage** | SD, SPI, I²C |
| **SATA** | 2× SATA 3.0 |
| **Security** | SEC security engine, 24 Gbit/s |
| **Acceleration** | DPAA2 engines for crypto, pattern matching, compression |
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
- [NXP LS2088A Product Page](https://www.nxp.com/products/LS2088A)
- [LS2088A Datasheet](https://www.nxp.com/docs/en/fact-sheet/LS2048A2088AFS.pdf)

---

## Boards with LS2088A

List of boards:

{{< taglist tag="LS2088A" style="cards" >}}
