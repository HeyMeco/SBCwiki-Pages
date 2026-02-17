---
weight: 13
title: NXP i.MX 952
#bookCollapseSection: true
soc-series:
- iMX9
soc:
- iMX952
tags: 
- SOC-NXP
- IMX-9
- iMX952
summary: NXP i.MX 952 ARM processor (Preproduction) - Quad Cortex-A55 + Cortex-M7 + Cortex-M33, Arm Mali 3D GPU (64 GFLOPS), eIQ Neutron NPU, LPDDR5 support, 2.5GbE + TSN, local dimming support, safe and secure for automotive and industrial edge.
---
# NXP i.MX 952

**Note:** This is a preproduction product. Specifications may change without notice.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **NXP i.MX 952 (Preproduction)**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Hexa-core: <br> 4× ARM Cortex-A55 <br> 1× ARM Cortex-M7 <br> 1× ARM Cortex-M33            |
| **RAM** | LPDDR5/LPDDR4X with inline ECC (IPED support on Octal SPI)                                                                                     |
| **GPU** | ARM Mali 3D GPU, 64 GFLOPS FP32, OpenGL ES 3.2, Vulkan 1.2, OpenCL 3.0 <br> 2D GPU               |
| **NPU** | NXP eIQ Neutron NPU for ML acceleration                                                                           |
| **ISP** | 500 MPixels/s, supports 4Kp60, 2× 4Kp30, 4× 1080p60 |
| **Display** | 4Kp30 or 3840×1440p60 MIPI-DSI (4-lane), up to 1080p60 LVDS (2× 4-lane or 1× 8-lane) <br> Local dimming support (512 zones) |
| **Camera** | 1× MIPI-CSI (4-lane or 2× 2-lane), up to 8× cameras with MIPI virtual channels |
| **Storage** | 3× SD 3.0/SDIO 3.0/eMMC 5.1, 1× Octal SPI with IPED |
| **Ethernet** | 1× 2.5GbE + 2× 1GbE (all with TSN support) |
| **USB** | 2× USB 2.0 |
| **PCIe** | 1× PCIe Gen 3.0 (1-lane) |
| **CAN** | 3× CAN-FD |
| **Audio** | 17-lane I²S TDM, 8× PDM mic, 2× MQS output, 5× SAI |
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
- [NXP i.MX 952 Product Page](https://www.nxp.com/products/i.MX-952)

---

## Boards with i.MX 952

List of boards:

{{< taglist tag="iMX952" style="cards" >}}
