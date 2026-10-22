---
weight: 18
title: NXP Layerscape LS1088A
#bookCollapseSection: true
soc-series:
- Layerscape
soc:
- LS1088A
tags: 
- SOC-NXP
- Layerscape
- LS1088A
summary: NXP Layerscape LS1088A networking processor - Octa-core Cortex-A53 (up to 1.6GHz), 3× PCIe Gen 3.0, 2× 10 Gigabit Ethernet + up to 8× Gigabit Ethernet, advanced packet processing and security.
---
# NXP Layerscape LS1088A

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
- [NXP LS1088A Product Page](https://www.nxp.com/products/LS1088A)
- [Layerscape Software Development Kit](https://www.nxp.com/design/design-center/software/embedded-software/linux-software-and-development-tools/layerscape-linux-distribution-poc:LAYERSCAPE-SDK)

---

## Boards with LS1088A

List of boards:

{{< taglist tag="LS1088A" style="cards" >}}
