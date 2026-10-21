---
weight: 16
title: Dragonwing Q2 / IQ2
soc-series:
- Dragonwing
soc:
- QRB2210
- QCS2290
- QCM2290
- Q-2390
- IQ-2390
tags:
- SOC-Qualcomm
- Dragonwing-Q
summary: Qualcomm Dragonwing Q2 and IQ2. QRB2210, QCS2290, and QCM2290 are quad Cortex-A53 parts. Q-2390 and IQ-2390 are one Cortex-A78 SoC in commercial and industrial grades.
---
# Dragonwing Q2 / IQ2

The Qualcomm Dragonwing Q2 series is the entry tier of Dragonwing IoT processors. It contains two different SoCs. QRB2210, QCS2290, and QCM2290 are the Agatti parts, with four Cortex-A53 cores. Q-2390 and IQ-2390 are a newer SoC, with one Cortex-A78 and three Cortex-A55 cores. IQ-2390 is the industrial grade of Q-2390. QRB2210 is the robotics part used on the Arduino Uno Q.

## General Specifications
{{% details title="Specs" open=true %}}

| **Part** | **CPU** | **GPU** | **Memory** | **AI** |
|----------|---------|---------|------------|--------|
| **QRB2210 / QCS2290 / QCM2290** | 4x Cortex-A53 @ 2.0 GHz<br>Codename Agatti | Adreno 702 @ 845 MHz | LPDDR4x @ 1804 MHz (2x 16-bit)<br>LPDDR3 @ 933 MHz (1x 32-bit) | — |
| **Q-2390 / IQ-2390** | 1x Cortex-A78 @ 1.9 GHz<br>3x Cortex-A55 @ 1.8 GHz | Adreno 704 @ 1.1 GHz | 2x 16-bit LPDDR4x @ 1.8 GHz<br>Up to 8 GB | Hexagon V66<br>Up to 1.1 INT8 TOPS |

{{% /details %}}

Agatti has a dual ISP: 13 MP + 13 MP, or 25 MP at 30 fps. The 2390 parts share a SiFive E61 RISC-V microcontroller at 600 MHz, dual ISPs, and 1080p30 H.264/H.265 decode and encode. Junction temperature for the 2390 parts is -30°C to 115°C. Qualcomm lists support until 2036. Operating systems are Android, Yocto Linux, Ubuntu, and Zephyr.

### Variant Differences:

- **QRB2210**: Robotics and IoT. No integrated LTE modem. Runs upstream Linux.
- **QCS2290**: Same application processor as QRB2210, aimed at POS, handhelds, tracking, and cameras.
- **QCM2290**: Adds an integrated 4G LTE modem.
- **Q-2390**: Commercial grade. Wi-Fi 5 and Bluetooth 5.1. The modem SKU adds 4G LTE and GPS.
- **IQ-2390** (orderable as IQ2390-AB): Industrial grade of Q-2390. 2x GbE with TSN, one PCIe Gen 2 lane, and Wi-Fi and Bluetooth on external chips. Aimed at HMIs, machine vision, gateways, small PLCs, scanners, panels, and energy equipment.

---

## Linux Support

### Mainline kernel

- **QRB2210 / QCS2290 / QCM2290**: Works, but not every feature is implemented. Driver support matrix is [Agatti](https://linux-msm.github.io/mainline-status/soc/agatti).
- **Q-2390 / IQ-2390**: No mainline status matrix lists these SKUs.

### Mesa GPU support

- [x] Adreno 702 is supported by [Freedreno](https://docs.mesa3d.org/drivers/freedreno.html)

---

## Resources

- [Q2 series](https://www.qualcomm.com/internet-of-things/products/q2-series)
- [IQ2 series](https://www.qualcomm.com/internet-of-things/products/iq2-series)
- [QRB2210](https://www.qualcomm.com/internet-of-things/products/q2-series/qrb2210)
- [QRB2210 data sheet](https://docs.qualcomm.com/bundle/publicresource/topics/80-30843-1)
- [IQ-2390](https://www.qualcomm.com/internet-of-things/products/iq2-series/iq-2390)
- [IQ-2390 product brief](https://docs.qualcomm.com/doc/87-A2425-1/87-A2425-1_REV_B_Qualcomm_Dragonwing_IQ-2390_Processor_Product_Brief.pdf)
- [Agatti mainline status](https://linux-msm.github.io/mainline-status/soc/agatti)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)

---

## Boards with Dragonwing Q2 / IQ2

List of boards:

{{< taglist tag="QRB2210" style="cards" >}}

{{< taglist tag="QCS2290" style="cards" >}}

{{< taglist tag="QCM2290" style="cards" >}}

{{< taglist tag="Q-2390" style="cards" >}}

{{< taglist tag="IQ-2390" style="cards" >}}
