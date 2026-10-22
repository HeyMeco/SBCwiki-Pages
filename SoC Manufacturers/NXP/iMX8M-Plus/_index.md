---
weight: 5
title: NXP i.MX 8M Plus
#bookCollapseSection: true
soc-series:
- iMX8M
soc:
- iMX8M-Plus
tags: 
- SOC-NXP
- IMX-8
- iMX8M-Plus
summary: NXP i.MX 8M Plus ARM processor - Quad-core Cortex-A53 (up to 1.8GHz) + Cortex-M7 (800MHz), GC7000UL GPU, 2.3 TOPS NPU for machine learning, dual camera ISP, 14nm FinFET process.
---
# NXP i.MX 8M Plus

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
- [NXP i.MX 8M Plus Product Page](https://www.nxp.com/products/i.MX8MPLUS)
- [i.MX 8M Plus Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX8MPIEC.pdf)

---

## Boards with i.MX 8M Plus

List of boards:

{{< taglist tag="iMX8M-Plus" style="cards" >}}
