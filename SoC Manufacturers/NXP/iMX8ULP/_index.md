---
weight: 8
title: NXP i.MX 8ULP
#bookCollapseSection: true
soc-series:
- iMX8ULP
soc:
- iMX8ULP
tags: 
- SOC-NXP
- IMX-8
- iMX8ULP
summary: NXP i.MX 8ULP ARM processor - Ultra-low power dual-core Cortex-A35 + dual Cortex-M33, Energy Flex architecture, 2D GPU, MIPI-DSI display, industrial and mobile applications.
---
# NXP i.MX 8ULP

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
- [NXP i.MX 8ULP Product Page](https://www.nxp.com/products/i.MX8ULP)
- [i.MX 8ULP Whitepaper](https://www.nxp.com/webapp/Download?colCode=IMX8ULPWP)

---

## Boards with i.MX 8ULP

List of boards:

{{< taglist tag="iMX8ULP" style="cards" >}}
