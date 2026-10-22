---
weight: 1
title: NXP i.MX 8
#bookCollapseSection: true
soc-series:
- iMX8
soc:
- iMX8
tags: 
- SOC-NXP
- IMX-8
- iMX8
summary: NXP i.MX 8 ARM processor - Advanced multicore processor with 2x Cortex-A72 (up to 1.3GHz) + 4x Cortex-A53 + 2x Cortex-M4F cores, dual GPU subsystems, 4K H.265 video decode, dual display controllers.
---
# NXP i.MX 8

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

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
- [NXP i.MX 8 Product Page](https://www.nxp.com/products/i.MX8)
- [i.MX 8 Family Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX8QM1P3AEC.pdf)

---

## Boards with i.MX 8

List of boards:

{{< taglist tag="iMX8" style="cards" >}}
