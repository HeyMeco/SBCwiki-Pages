---
weight: 11
title: NXP i.MX 94
#bookCollapseSection: true
soc-series:
- iMX9
soc:
- iMX94
tags: 
- SOC-NXP
- IMX-9
- iMX94
summary: NXP i.MX 94 ARM processor (Preproduction) - Quad Cortex-A55 + dual Cortex-M33 + dual Cortex-M7 cores, NPU, 3-port TSN switch with 2.5GbE support, safe and secure connectivity for industrial and automotive applications.
---
# NXP i.MX 94

**Note:** This is a preproduction product. Specifications may change without notice.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 94 (Preproduction)**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Hexa-core: <br> 4× ARM Cortex-A55 <br> 2× ARM Cortex-M33 <br> 2× ARM Cortex-M7            |
| **RAM** | LPDDR4 with inline ECC                                                                                     |
| **GPU** | 2D GPU, 1 GFLOPS               |
| **NPU** | Integrated NPU for ML acceleration                                                                           |
| **Display** | 1080p60 LVDS (4-lane) |
| **Storage** | 3× SD/SDIO 3.0/eMMC 5.1, 1× Octal SPI |
| **Ethernet** | 3-port TSN switch (2× 2.5GbE, 1× 1GbE) + 2× 1GbE with TSN |
| **USB** | 1× USB 2.0, 1× USB 3.0 |
| **PCIe** | 2× PCIe Gen 3.0 (1-lane) |
| **CAN** | 5× CAN-FD |
| **Audio** | 3× I²S, PDM mic |
| **Security** | EdgeLock secure enclave |

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [ ] Works but not all features are implemented.

Preproduction SoC - mainline support to be added upon production release

### Vendor BSP
- NXP will provide [linux-imx kernel](https://github.com/nxp-imx/linux-imx) and [Yocto-based BSP](https://www.nxp.com/design/design-center/software/embedded-software/i-mx-software/embedded-linux-for-i-mx-applications-processors:IMXLINUX) upon production release

---

## Documentation
- [NXP i.MX 94 Product Page](https://www.nxp.com/products/i.MX94)

---

## Boards with i.MX 94

List of boards:

{{< taglist tag="iMX94" style="cards" >}}
