---
weight: 12
title: Dragonwing Q6 / IQ6
soc-series:
- Dragonwing
soc:
- Q-6690
- QCM6490
- QCS6490
- QCS610
- QCS6125
- IQ-615
tags:
- SOC-Qualcomm
- Dragonwing-Q
summary: Qualcomm Dragonwing Q6 and IQ6. Commercial parts include Q-6690, QCS6490, QCM6490, QCS610, and QCS6125, rated up to 12 TOPS. IQ-615 is the industrial part.
---
# Dragonwing Q6 / IQ6

The Qualcomm Dragonwing Q6 series is the commercial tier for retail, logistics, healthcare, warehousing, and manufacturing. Qualcomm rates that tier at up to 12 TOPS, with Wi-Fi 6E and optional 5G. IQ6 is the industrial tier for HMIs, edge controllers, gateways, handhelds, and machine vision. [QCS6490 / QCM6490](/docs/soc-manufacturers/qualcomm/dragonwing-6490/) has its own page. IQ-615 is the industrial part, with a Kryo 460 cluster of Cortex-A76 and Cortex-A55 cores and a Spectra 230 ISP.

## General Specifications
{{% details title="Specs" open=true %}}

| **Part** | **CPU** | **GPU** | **Memory** | **Notes** |
|----------|---------|---------|------------|-----------|
| **Q-6690** | 1x Cortex-A715 @ 2.9 GHz<br>3x Cortex-A715 @ 2.7 GHz<br>4x Cortex-A510 @ 2.0 GHz<br>4 nm | Adreno @ 1.15 GHz | 2x16-bit LPDDR5 @ 3200 MHz | Hexagon, 6 TOPS. Android. Wi-Fi 7 and Wi-Fi 6E, 2x2. Bluetooth 5.4 and Bluetooth 6.0 |
| **[QCS6490 / QCM6490](/docs/soc-manufacturers/qualcomm/dragonwing-6490/)** | Cortex-A78 and Cortex-A55, 6 nm | Adreno 643 | LPDDR5 / LPDDR4x | Full specifications are on the [chip page](/docs/soc-manufacturers/qualcomm/dragonwing-6490/) |
| **QCS610** | 2x Cortex-A76 up to 2.2 GHz<br>6x Cortex-A55<br>11 nm | Adreno 612 | LPDDR4x @ 1804 MHz | Hexagon 685. Android and Linux. Wi-Fi 5 and Wi-Fi 4, 1x1. Bluetooth 5.0. 10-year longevity |
| **QCS6125** | 4x Cortex-A73 @ 2.0 GHz<br>4x Cortex-A53 @ 1.8 GHz<br>11 nm | Adreno 610 | LPDDR4x @ 1804 MHz (2x16)<br>LPDDR3 @ 933 MHz (1x32) | Hexagon 686. Snapdragon X12 LTE modem. Android and Linux. Wi-Fi 5 1x1. Bluetooth 5.0 |
| **IQ-615** | 2x Cortex-A76 and 6x Cortex-A55, up to 1.9 GHz | Adreno 612 @ 845 MHz | 2x 16-bit LPDDR4x @ 1555 MHz<br>Up to 8 GB | Hexagon V66 @ 1.0 GHz. Yocto Linux and Ubuntu. Industrial grade |

{{% /details %}}

### Variant Differences:

- **Q-6690**: Newer 4 nm part. Two DisplayPort outputs with multi-stream transport. 167 GPIOs.
- **QCS610**: USB 2.0, USB 3.1, and RGMII Ethernet. Two displays. The Cortex-A76 cluster is the same generation as the Talos platform ([SM6150 / QCS615](https://linux-msm.github.io/mainline-status/soc/talos)). QCS610 itself is not listed on that matrix.
- **QCS6125**: Adds the integrated X12 LTE modem that QCS610 does not have.
- **IQ-615**: Industrial grade. Spectra 230, Adreno VPU 443 (4K60 H.265/H.264/VP9 decode, 1080p60 H.265/H.264 encode), up to six cameras, and three displays. RGMII Ethernet, USB, PCIe, and Bluetooth 5.3. Junction temperature is -40°C to 105°C. Qualcomm lists support until 2038.

---

## Linux Support

### Mainline kernel

- **QCS6490 / QCM6490**: Fully supported. Matrix is on the [chip page](/docs/soc-manufacturers/qualcomm/dragonwing-6490/).
- **Q-6690, QCS610, QCS6125, IQ-615**: No mainline status matrix lists these SKUs. QCS610 and IQ-615 use the same Cortex-A76 generation as [Talos (SM6150 / QCS615)](https://linux-msm.github.io/mainline-status/soc/talos).

### Qualcomm Linux

- [x] IQ-615 lists Yocto Linux and Ubuntu

---

## Resources

- [Q6 series](https://www.qualcomm.com/internet-of-things/products/q6-series)
- [IQ6 series](https://www.qualcomm.com/internet-of-things/products/iq6-series)
- [IQ-615](https://www.qualcomm.com/internet-of-things/products/iq6-series/iq-615)
- [Q-6690 product brief](https://docs.qualcomm.com/doc/87-91418-1/87-91418-1_REV_A_Qualcomm_Dragonwing_Q-6690_Processor_Product_Brief.pdf)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)

---

## Boards with Dragonwing Q6 / IQ6

List of boards:

{{< taglist tag="Q-6690" style="cards" >}}

{{< taglist tag="QCS6490" style="cards" >}}

{{< taglist tag="QCM6490" style="cards" >}}

{{< taglist tag="QCS610" style="cards" >}}

{{< taglist tag="QCS6125" style="cards" >}}

{{< taglist tag="IQ-615" style="cards" >}}
