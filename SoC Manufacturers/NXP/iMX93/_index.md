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

| **SoC** | **NXP i.MX 93**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Dual-core: <br> 2× ARM Cortex-A55 (up to 1.7GHz) <br> 1× ARM Cortex-M33 (up to 250MHz)            |
| **RAM** | LPDDR4 with inline ECC                                                                                     |
| **GPU** | 2D GPU               |
| **NPU** | ARM Ethos-U65 microNPU, 256 MACs @ 1.0GHz, 8-bit/16-bit integer                                                                           |
| **ISP** | 1080p60 camera processing |
| **Display** | 1080p60 MIPI-DSI (4-lane), 720p60 LVDS (4-lane), 24-bit parallel RGB |
| **Camera** | 1080p60 MIPI-CSI (2-lane), 8-bit parallel YUV/RGB |
| **Storage** | 3× SD/SDIO 3.0/eMMC 5.1, 1× Octal SPI |
| **Ethernet** | 2× Gigabit Ethernet (1× with TSN support) |
| **USB** | 2× USB 2.0 |
| **Audio** | 7× I²S, SPDIF, PDM mic, MQS output |
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
- [NXP i.MX 93 Product Page](https://www.nxp.com/products/processors-and-microcontrollers/arm-processors/i-mx-applications-processors/i-mx-9-processors/i-mx-93-applications-processor-family-arm-cortex-a55-ml-acceleration-power-efficient-mpu:i.MX93)
- [i.MX 93 Datasheet](https://www.nxp.com/docs/en/data-sheet/IMX93AEC.pdf)

---

## Boards with i.MX 93

List of boards:

{{< taglist tag="iMX93" style="cards" >}}
