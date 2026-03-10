---
weight: 1
title: Dragonwing IQ9 Series
#bookCollapseSection: true
soc-series:
- Dragonwing
soc:
- QCS9100
- QCS9075
tags: 
- SOC-Qualcomm
summary: Qualcomm Dragonwing IQ9 Series (QCS9100, QCS9075) premium industrial IoT SoCs featuring up to 100 dense TOPS AI performance, SIL3-capable safety island, and support for up to 16 cameras.
---
# Dragonwing IQ9 Series

The Qualcomm Dragonwing IQ9 series represents the premium tier of industrial IoT solutions, offering massive AI compute power (up to 100 dense TOPS) and high-end multimedia capabilities.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **QCS9075 / QCS9100** - Codename: Lemans |
|---------|-----------------------|
| **CPU** | **Octa-Core Kryo Gen 6**:<br>Up to 2.36 GHz |
| **RAM** | 6x16bit LPDDR5 @ 3200 MHz<br>- Up to 36 GB with inline ECC |
| **GPU** | Adreno 663 GPU @ 800 MHz |
| **VPU** | **Decode**: 1x 8K60, 2x 8K30, 4x 4K60<br>- AV1, H.264, H.265, VP9, MPEG2<br>**Encode**: 2x 4K60, 4x 4K30<br>- H.264, H.265 |
| **NPU** | Hexagon:<br>- 100 dense TOPS<br>- Llama 2 7B: 22 tokens/sec |
| **Other** | 8x CAN-FD, 2x 2.5 GbE |

{{% /details %}}

### Also known as

- SA8775P

### Variant Differences

- QCS9075-**AC**: 50 dense TOPS NPU (instead of 100 TOPS) and 530 MHz GPU (instead of 800 MHz)
- QCS**9100**: Features a dedicated **Safety Island** with planned support for **SIL3** safety certification.

---

## Linux Support

### Mainline Kernel

- [ ] With 6.18 it does not boot yet.
- [Mainline Driver Status Matrix](https://linux-msm.github.io/mainline-status/soc/lemans)

### Qualcomm-Linux
- [x] Supported

## Resources

- [Qualcomm Introduces Industrial-Grade IQ Series](hhttps://www.qualcomm.com/news/releases/2024/10/qualcomm-introduces-industrial-grade-iq-series-and-iot-solutions)
- [IQ9 Product Brief](https://docs.qualcomm.com/doc/87-83840-1/87-83840-1_REV_A_Qualcomm_IQ9_Series_Product_Brief.pdf)

---

## Boards with Dragonwing IQ9

List of boards:

{{< taglist tag="QCS9100" style="cards" >}}

{{< taglist tag="QCS9075" style="cards" >}}



