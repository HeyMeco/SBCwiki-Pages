---
weight: 10
title: NXP i.MX 93
#bookCollapseSection: true
soc-series:
- iMX9
soc:
- iMX93
tags: 
- SOC-NXP
- IMX-9
- iMX93
summary: NXP i.MX 93 ARM processor - Dual Cortex-A55 cores (up to 1.7GHz) + Cortex-M33, 2D GPU, Arm Ethos-U65 microNPU, dual Gigabit Ethernet with TSN, ML acceleration for automotive and industrial IoT.
---
# NXP i.MX 93

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
- [NXP i.MX 93 Product Page](https://www.nxp.com/products/processors-and-microcontrollers/arm-processors/i-mx-applications-processors/i-mx-9-processors/i-mx-93-applications-processor-family-arm-cortex-a55-ml-acceleration-power-efficient-mpu:i.MX93)
- [i.MX 93 Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX93AEC.pdf)

---

## Boards with i.MX 93

List of boards:

{{< taglist tag="iMX93" style="cards" >}}
