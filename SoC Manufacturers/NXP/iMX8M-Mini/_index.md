---
weight: 3
title: NXP i.MX 8M Mini
#bookCollapseSection: true
soc-series:
- iMX8M
soc:
- iMX8M-Mini
tags: 
- SOC-NXP
- IMX-8
- iMX8M-Mini
summary: NXP i.MX 8M Mini ARM processor - Quad-core Cortex-A53 (up to 1.8GHz) + Cortex-M4, GCNanoUltra GPU, 1080p60 H.265/VP9 video decode, 14nm FinFET process.
---
# NXP i.MX 8M Mini

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
- [NXP i.MX 8M Mini Product Page](https://www.nxp.com/products/i.MX8MMINI)
- [i.MX 8M Mini Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX8MMCEC.pdf)

---

## Boards with i.MX 8M Mini

List of boards:

{{< taglist tag="iMX8M-Mini" style="cards" >}}
