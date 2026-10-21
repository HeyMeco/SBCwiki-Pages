---
weight: 15
title: Dragonwing Q4 Series
soc-series:
- Dragonwing
soc:
- Q-4390
- QCM4490
- QCS4490
- QCS4290
- QCM4290
- QCS410
- QRB4210
tags:
- SOC-Qualcomm
- Dragonwing-Q
summary: Qualcomm Dragonwing Q4 processors for handhelds, retail, cameras, and robots, from the 4 nm Cortex-A78 QCS4490 down to Cortex-A73 parts such as QRB4210.
---
# Dragonwing Q4 Series

The Qualcomm Dragonwing Q4 series is for handhelds, smart retail, edge cameras, healthcare devices, and small robots. Qualcomm's family comparison lists the series at 1.1 TOPS. The active parts are octa-core Cortex-A78, Cortex-A76, and Cortex-A73 designs, and the top of the series adds Wi-Fi 6E with optional 5G.

## General Specifications
{{% details title="Specs" open=true %}}

| **Part** | **CPU** | **GPU** | **Memory** | **Process** |
|----------|---------|---------|------------|-------------|
| **Q-4390** | 2x Cortex-A78 up to 2.2 GHz<br>6x Cortex-A55 | Adreno 613 @ 738 MHz | LPDDR5 @ 2750 MHz and LPDDR4x @ 2100 MHz, 2x16 | 4 nm |
| **QCM4490 / QCS4490** | 2x Cortex-A78 up to 2.4 GHz<br>6x Cortex-A55 | Adreno 613 @ 1.01 GHz | LPDDR5 @ 3200 MHz and LPDDR4x @ 2100 MHz, 2x16 | 4 nm |
| **QCS4290 / QCM4290** | 4x Cortex-A73 up to 2.0 GHz<br>4x Cortex-A53 | Adreno 610 | LPDDR4x @ 1866 MHz (2x16)<br>LPDDR3 @ 933 MHz (1x32) | 11 nm |
| **QCS410** | 2x Cortex-A76 up to 2.2 GHz<br>6x Cortex-A55 | Adreno 612 | LPDDR4x @ 1804 MHz | 11 nm |
| **QRB4210** | 4x Cortex-A73 @ 2.0 GHz<br>4x Cortex-A53 @ 1.8 GHz | Adreno 610 @ 950 MHz | LPDDR4x @ 1866 MHz (2x16)<br>LPDDR3 @ 933 MHz (1x32) | 11 nm |

{{% /details %}}

### Variant Differences:

- **Q-4390**: Android. Wi-Fi 6E 2x2 and Bluetooth 5.2. One PCIe Gen3 lane and USB 3.1. One display.
- **QCS4490**: Same class as Q-4390 with a higher CPU and GPU clock. Android, Wi-Fi 6E, Bluetooth 5.2. 7-year longevity.
- **QCM4490**: Modem SKU of QCS4490.
- **QCS4290**: Android and Linux. Wi-Fi 5, Wi-Fi 4, and Wi-Fi 6-ready, Bluetooth 5.1. Hexagon 683 with dual HVX. Pin compatible with QCS2290. 3rd gen AI Engine.
- **QCM4290**: Same Cortex-A73 platform as QCS4290, with an integrated modem. Bluetooth 5.0.
- **QCS410**: Android and Linux. Wi-Fi 5 and Wi-Fi 4 at 1x1, Bluetooth 5.0. USB 2.0, USB 3.1, and RGMII Ethernet. Hexagon 685. 10-year longevity. Same Cortex-A76 cluster as QCS610 in the [Q6 series](/docs/soc-manufacturers/qualcomm/dragonwing-q6/).
- **QRB4210**: Robotics part. Linux. Wi-Fi 4 1x1 and Bluetooth 5.0. Hexagon dual HVX at 1.0 GHz. About 1 TOPS.

---

## Linux Support

### Mainline kernel

- **QCS4290 / QCM4290 / QRB4210**: Listed on the [Kamorta matrix](https://linux-msm.github.io/mainline-status/soc/kamorta), with SM6115.
- **Q-4390, QCS4490, QCM4490, QCS410**: No mainline status matrix lists these SKUs. The related [SM4450 matrix](https://linux-msm.github.io/mainline-status/soc/sm4450) does not name the 4490 or Q-4390 parts.

Vendor operating systems are Android and Linux on the Cortex-A73 and Cortex-A76 parts. Q-4390, QCS4490, and QCM4490 are listed as Android.

---

## Resources

- [Q4 series](https://www.qualcomm.com/internet-of-things/products/q4-series)
- [QRB4210](https://www.qualcomm.com/internet-of-things/products/q4-series/qrb4210)
- [QCS4290](https://www.qualcomm.com/internet-of-things/products/q4-series/qcs4290)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)

---

## Boards with Dragonwing Q4

List of boards:

{{< taglist tag="QCS4490" style="cards" >}}

{{< taglist tag="QCM4490" style="cards" >}}

{{< taglist tag="Q-4390" style="cards" >}}

{{< taglist tag="QCS4290" style="cards" >}}

{{< taglist tag="QCM4290" style="cards" >}}

{{< taglist tag="QCS410" style="cards" >}}

{{< taglist tag="QRB4210" style="cards" >}}
