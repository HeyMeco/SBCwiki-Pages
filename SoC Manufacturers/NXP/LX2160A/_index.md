---
weight: 20
title: NXP Layerscape LX2160A
#bookCollapseSection: true
soc-series:
- Layerscape
soc:
- LX2160A
tags: 
- SOC-NXP
- Layerscape
- LX2160A
summary: NXP Layerscape LX2160A flagship networking processor - 16× Cortex-A72 cores (up to 2.2GHz), 6× PCIe Gen 3.0, up to 100 Gigabit Ethernet with 16× ports, 122 Gbit/s L2 switch, 50 Gbit/s security offload, 25 GHz SerDes.
---
# NXP Layerscape LX2160A

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP Layerscape LX2160A**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | 16-core (also available as 8 or 12-core variants): <br> 16× ARM Cortex-A72 (up to 2.2GHz)            |
| **RAM** | DDR4                                                                                     |
| **Ethernet** | Up to 16× Ethernet ports with speeds of 1, 2.5, 10, 25, 40, 50, and 100 Gbit/s |
| **L2 Switch** | 122 Gbit/s L2 switching capability |
| **PCIe** | 6× PCIe Gen 3.0 (24 lanes total) |
| **SerDes** | 24× 25 GHz SerDes lanes |
| **Storage** | SD, SPI, I²C |
| **SATA** | 4× SATA 3.0 |
| **Security** | SEC security engine, 50 Gbit/s offload capability |
| **Compression** | 100 Gbit/s compression engine |
| **Acceleration** | DPAA2 acceleration engines for crypto, pattern matching, compression |
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
- [NXP LX2160A Product Page](https://www.nxp.com/products/LX2160A)
- [LX2160A Fact Sheet](https://www.nxp.com/docs/en/fact-sheet/LX2160AFS.pdf)

---

## Boards with LX2160A

List of boards:

{{< taglist tag="LX2160A" style="cards" >}}
