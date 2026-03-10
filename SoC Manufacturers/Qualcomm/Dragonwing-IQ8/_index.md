---
weight: 2
title: Dragonwing IQ8 Series
#bookCollapseSection: true
soc-series:
- Dragonwing
soc:
- QCS8300
- QCS8275
tags: 
- SOC-Qualcomm
summary: Qualcomm Dragonwing IQ8 Series (QCS8300, QCS8275) industrial IoT SoCs featuring up to 40 TOPS AI performance, SIL3-compliant safety island, and support for up to 12 cameras.
---
# Dragonwing IQ8 Series

The Qualcomm Dragonwing IQ8 series is designed for mid-tier industrial IoT applications, balancing high-performance computing with integrated safety features.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **QCS8275 / QCS8300** - Codename: Monaco |
|---------|-----------------------|
| **CPU** | **Octa-core Kryo Gen 6**:<br>2x Kryo Gold Prime @ 2.35 GHz<br>2x Kryo Gold @ 2.1 GHz<br>4x Kryo Silver @ 1.95 GHz |
| **RAM** | 4x16-bit LPDDR5/5x @ 3200 MHz<br>- Up to 32 GB with inline ECC |
| **GPU** | Adreno 623 GPU |
| **VPU** | **Decode:** 4K@135fps <br> - AV1, H.265, H.264, VP9<br>**Encode:** 4K@85fps<br>- H.264, H.265 |
| **NPU** | Hexagon Tensor Processor:<br>- 20-40 INT8 TOPS (Dense) |
| **Other** | 4x CAN FD, 1x GbE |

{{% /details %}}

### Variant Differences:

- **QCS8275**: AI performance scalable between 20-40 TOPS.
- **QCS8300**: Features a dedicated **Safety Island** with planned support for **SIL3** safety certification; AI performance up to 40 TOPS guaranteed.

---

## Linux Support

### Mainline Kernel

- [ ] With 6.18 - Untested
- [Mainline Driver Status Matrix](https://linux-msm.github.io/mainline-status/soc/monaco)

### Qualcomm-Linux
- [x] Supported

## Resources

- [Qualcomm Introduces Industrial-Grade IQ Series](hhttps://www.qualcomm.com/news/releases/2024/10/qualcomm-introduces-industrial-grade-iq-series-and-iot-solutions)
- [IQ8 Product Brief](https://docs.qualcomm.com/doc/87-83839-1/87-83839-1_REV_A_Qualcomm_IQ8_Series_Product_Brief________.pdf)

## Boards with Dragonwing IQ8

List of boards:

{{< taglist tag="QCS8300" style="cards" >}}

{{< taglist tag="QCS8275" style="cards" >}}

