---
weight: 17
title: NXP Layerscape LS1046A
#bookCollapseSection: true
soc-series:
- Layerscape
soc:
- LS1046A
tags: 
- SOC-NXP
- Layerscape
- LS1046A
summary: NXP Layerscape LS1046A networking processor - Quad Cortex-A72 cores (up to 1.8GHz), 3× PCIe Gen 3.0, 2× 10 Gigabit Ethernet + up to 5× Gigabit Ethernet, SEC security engine with 10 Gbit/s throughput.
---
# NXP Layerscape LS1046A

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
- [NXP LS1046A Product Page](https://www.nxp.com/products/LS1046A)
- [Layerscape Software Development Kit](https://www.nxp.com/design/design-center/software/embedded-software/linux-software-and-development-tools/layerscape-linux-distribution-poc:LAYERSCAPE-SDK)

---

## Boards with LS1046A

List of boards:

{{< taglist tag="LS1046A" style="cards" >}}
