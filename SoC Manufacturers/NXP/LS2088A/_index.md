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
- [NXP LS2088A Product Page](https://www.nxp.com/products/LS2088A)
- [LS2088A Datasheet](https://www.nxp.com/docs/en/fact-sheet/LS2048A2088AFS.pdf)

---

## Boards with LS2088A

List of boards:

{{< taglist tag="LS2088A" style="cards" >}}
