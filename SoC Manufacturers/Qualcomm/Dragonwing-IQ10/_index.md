---
weight: 1
title: Dragonwing IQ10 Series
soc-series:
- Dragonwing
soc:
- IQ-10800
tags:
- SOC-Qualcomm
- Dragonwing-IQ
summary: Qualcomm Dragonwing IQ10 robotics processors, with up to 18 custom Oryon cores and a Hexagon NPU rated at 700 sparse TOPS.
---
# Dragonwing IQ10 Series

The Qualcomm Dragonwing IQ10 series is the top of the industrial IQ family, aimed at humanoid robots, advanced AMRs, collaborative robots, and edge AI automation. The CPU is Qualcomm's custom Oryon design. Orderable parts are IQ-10800MD-AA and IQ-10800MD-AD.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **IQ-10800** |
|---------|----------------|
| **CPU** | Up to 18x Oryon up to 3.014 GHz<br>Custom Qualcomm cores |
| **RAM** | 16x 16-bit LPDDR5x, ECC, up to 128 GB<br>IQ-10800MD-AA: 64 GB<br>IQ-10800MD-AD: 32 GB |
| **GPU** | Primary Adreno up to 1.0 GHz<br>Secondary Adreno up to 1.1 GHz |
| **NPU** | Hexagon, 700 INT8 sparse TOPS<br>350 dense TOPS |
| **OS** | Linux and Ubuntu |

{{% /details %}}

### Variant Differences:

- **IQ-10800MD-AA**: 64 GB DDR.
- **IQ-10800MD-AD**: 32 GB DDR.
- Both parts share the Oryon CPU, dual Adreno GPUs, and the Hexagon NPU. The platform adds a safety island with planned support up to SIL3, up to 20 cameras, 4x PCIe Gen 5, and 2x 10GbE with TSN. The product brief lists an ambient range of -40°C to 85°C. The series catalog lists -40°C to 125°C, with support until 2038.

---

## Linux Support

### Mainline kernel

- [ ] No mainline status matrix lists IQ-10800 yet

### Qualcomm Linux

- [x] Linux and Ubuntu are the operating systems Qualcomm lists for this series

---

## Resources

- [IQ10 series](https://www.qualcomm.com/internet-of-things/products/iq10-series)
- [IQ10 series platform product brief](https://docs.qualcomm.com/doc/87-A2811-1/87-A2811-1_REV_A_Qualcomm_Dragonwing_IQ10_Series_Platform_Product_Brief.pdf)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)

---

## Boards with Dragonwing IQ10

List of boards:

{{< taglist tag="IQ-10800" style="cards" >}}
