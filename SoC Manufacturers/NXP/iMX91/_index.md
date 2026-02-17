---
weight: 9
title: NXP i.MX 91
#bookCollapseSection: true
soc-series:
- iMX9
soc:
- iMX91
tags: 
- SOC-NXP
- IMX-9
- iMX91
summary: NXP i.MX 91 ARM processor - Single Cortex-A55 core (up to 1.4GHz) with optional Cortex-M33, EdgeLock secure enclave, dual Gigabit Ethernet with TSN, energy-efficient design for IoT and industrial applications.
---
# NXP i.MX 91

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 91**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Single-core: <br> 1× ARM Cortex-A55 (up to 1.4GHz) <br> Optional: 1× ARM Cortex-M33            |
| **RAM** | LPDDR4 (up to 2.4 GT/s) with inline ECC                                                                                     |
| **Display** | 24-bit parallel RGB/YUV display interface |
| **Camera** | 8-bit parallel RGB/YUV camera interface |
| **Storage** | 3× SD/SDIO 3.0/eMMC 5.1, 1× Octal SPI |
| **Ethernet** | 2× Gigabit Ethernet (1× with TSN support) |
| **USB** | 2× USB 2.0 (dual mode with Type-C support) |
| **PCIe** | PCIe Gen 3.0 |
| **Audio** | 3× SAI, 4× I²S TDM, 8-channel PDM microphone input, SPDIF |
| **Security** | EdgeLock secure enclave |

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
- [NXP i.MX 91 Product Page](https://www.nxp.com/products/i.MX91)
- [i.MX 91 Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX91IEC.pdf)

---

## Boards with i.MX 91

List of boards:

{{< taglist tag="iMX91" style="cards" >}}
