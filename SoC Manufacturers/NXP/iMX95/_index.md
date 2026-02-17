---
weight: 12
title: NXP i.MX 95
#bookCollapseSection: true
soc-series:
- iMX9
soc:
- iMX95
tags: 
- SOC-NXP
- IMX-9
- iMX95
summary: NXP i.MX 95 ARM processor (Preproduction) - Hexa-core Cortex-A55 + Cortex-M7 + Cortex-M33, Arm Mali 3D GPU (64 GFLOPS), eIQ Neutron NPU, LPDDR5 support, 10GbE + TSN, safe and secure for automotive and industrial edge.
---
# NXP i.MX 95

**Note:** This is a preproduction product. Specifications may change without notice.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 95 (Preproduction)**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Octa-core: <br> 6× ARM Cortex-A55 (32KB I-cache, 32KB D-cache, 64KB L2, 512KB L3 with ECC) <br> 1× ARM Cortex-M7 (32KB I-cache, 32KB D-cache, 512KB TCM with ECC) <br> 1× ARM Cortex-M33 (16KB I-cache, 16KB D-cache, 256KB OCRAM with ECC)            |
| **RAM** | LPDDR5/LPDDR4X (up to 6.4GT/s x32) with inline ECC                                                                                     |
| **GPU** | ARM Mali 3D GPU, 64 GFLOPS FP32, OpenGL ES 3.2, Vulkan 1.2, OpenCL 3.0 <br> 2D GPU               |
| **NPU** | NXP eIQ Neutron NPU for ML acceleration                                                                           |
| **ISP** | 500 MPixels/s, supports 4Kp60, 2× 4Kp30, 4× 1080p60, 8× 1080p30 |
| **Display** | 4Kp30 or 3840×1440p60 MIPI-DSI (4-lane), up to 1080p60 LVDS (2× 4-lane or 1× 8-lane) |
| **Camera** | 2× MIPI-CSI (4-lane), up to 8× cameras with MIPI virtual channels |
| **Storage** | 3× SD 3.0/SDIO 3.0/eMMC 5.1, 1× Octal SPI |
| **Ethernet** | 10GbE + 2× 1GbE (all with TSN support) |
| **USB** | 1× USB 3.0, 2× USB 2.0 |
| **PCIe** | 2× PCIe Gen 3.0 (1-lane) |
| **CAN** | 5× CAN-FD |
| **Audio** | 17-lane I²S TDM, SPDIF, 8× PDM mic, 2× MQS output, 5× SAI |
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
- [NXP i.MX 95 Product Page](https://www.nxp.com/products/i.MX95)
- [i.MX 95 Press Release](https://www.nxp.com/company/about-nxp/newsroom/nxps-new-i-mx-95-family-of-application-processors-delivers-safe-secure-and-scalable-ai-enabled-edge-platforms:NW-NXP-NEW-IMX95-FAMILY-OF-APPLICATIONS)

---

## Boards with i.MX 95

List of boards:

{{< taglist tag="iMX95" style="cards" >}}
