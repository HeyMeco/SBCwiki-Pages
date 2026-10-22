---
weight: 14
title: NXP Layerscape LS1012A
#bookCollapseSection: true
soc-series:
- Layerscape
soc:
- LS1012A
tags: 
- SOC-NXP
- Layerscape
- LS1012A
summary: NXP Layerscape LS1012A networking processor - Single Cortex-A53 core (up to 1GHz), PCIe Gen 2.0, up to 2× Gigabit Ethernet, compact form factor for power-constrained networking and IoT applications.
---
# NXP Layerscape LS1012A

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

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
- [NXP LS1012A Product Page](https://www.nxp.com/products/LS1012A)
- [Layerscape Software Development Kit](https://www.nxp.com/design/design-center/software/embedded-software/linux-software-and-development-tools/layerscape-linux-distribution-poc:LAYERSCAPE-SDK)

---

## Boards with LS1012A

List of boards:

{{< taglist tag="LS1012A" style="cards" >}}
