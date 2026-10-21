---
weight: 10
title: Dragonwing Q8 / IQ8
soc-series:
- Dragonwing
soc:
- Q-8750
- QCM8550
- QCS8550
- QCS8250
- SDA845
- QCS8300
- QCS8275
tags:
- SOC-Qualcomm
- Dragonwing-Q
summary: Qualcomm Dragonwing Q8 and IQ8. Commercial parts run from the Oryon Q-8750 at 77 dense TOPS down to SDA845. IQ8 is the industrial Monaco SoC, QCS8275 and QCS8300, at up to 40 dense TOPS.
---
# Dragonwing Q8 / IQ8

The Qualcomm Dragonwing Q8 series is the top of the commercial Q family. Qualcomm rates it at up to 77 TOPS, for smart displays, video conferencing, wearables, body and motion cameras, and set-top boxes. IQ8 is the industrial series, codename Monaco, for fleet cameras, machine vision, gateways, PLCs, and robotics. These parts do not share one CPU. Q-8750 uses Qualcomm's custom Oryon cores. QCS8550 and QCM8550 are the SM8550 cluster. QCS8250 and SDA845 are older Cortex-A77 and Cortex-A75 designs. QCS8275 and QCS8300 are Kryo Gen 6.

## General Specifications
{{% details title="Specs" open=true %}}

| **Part** | **CPU** | **GPU** | **Memory** | **AI** |
|----------|---------|---------|------------|--------|
| **Q-8750** | 8x Oryon up to 4.32 GHz<br>Custom Qualcomm cores, 3 nm | Adreno 830 @ 1.1 GHz | LPDDR5x @ 4800 MHz<br>4x 16-bit, up to 24 GB | Hexagon V79<br>77 dense TOPS |
| **QCM8550 / QCS8550** | 1x Cortex-X3 @ 3.2 GHz<br>2x Cortex-A715 @ 2.8 GHz<br>2x Cortex-A710 @ 2.8 GHz<br>3x Cortex-A510 @ 2.0 GHz<br>4 nm | Adreno 740 @ 680 MHz | LPDDR5x @ 4200 MHz | — |
| **QCS8250** | 4x Cortex-A77 @ 2.85 GHz<br>4x Cortex-A55 @ 1.8 GHz<br>7 nm | Adreno 650 | Quad-channel PoP LPDDR5/LPDDR4x @ 2750 MHz | Hexagon V66Q @ 1.5 GHz<br>15 TOPS |
| **SDA845** | 4x Cortex-A75 @ 2.8 GHz<br>4x Cortex-A55 @ 1.8 GHz<br>10 nm | Adreno 630 | LPDDR4x @ 1866 MHz | Hexagon 685 |
| **QCS8275 / QCS8300** | Octa-core Kryo Gen 6<br>2x Kryo Gold Prime @ 2.35 GHz<br>2x Kryo Gold @ 2.1 GHz<br>4x Kryo Silver @ 1.95 GHz<br>Codename Monaco | Adreno 623 | 4x 16-bit LPDDR5/5x @ 3200 MHz<br>Up to 32 GB with inline ECC | Hexagon<br>20–40 dense INT8 TOPS |

{{% /details %}}

### Variant Differences:

- **Q-8750**: Android 15+ and Yocto Linux. Wi-Fi 7 and Bluetooth 6.0 need companion chips. Display outputs are 2x MIPI (up to 8K60) and 8x DisplayPort. Video decode goes to 8K60, encode to 8K30. Up to 12 cameras with triple 48 MP ISPs.
- **QCM8550**: Same application processor as QCS8550, plus a Snapdragon X70 5G modem. Android, Linux, and Ubuntu. Wi-Fi 7 2x2 and Bluetooth 5.3. Four displays. 10-year longevity.
- **QCS8550**: The standalone version of that processor, without the X70 modem.
- **QCS8250**: Android. Wi-Fi 6 2x2 and Bluetooth 5.1. Three displays. 15-year longevity.
- **SDA845**: The IoT SKU of SDM845. Wi-Fi 5 and Bluetooth 5.0.
- **QCS8275**: Industrial grade. AI performance scales from 20 to 40 dense TOPS. Decode is 4K135 for AV1, H.265, H.264, and VP9. Encode is 4K85 for H.264 and H.265. 4x CAN FD and 1x GbE. Yocto Linux and Ubuntu. Rated -40°C to 125°C, supported until 2038.
- **QCS8300**: Same Monaco SoC as QCS8275, with a safety island and planned SIL3 support. AI performance is 40 dense TOPS.

---

## Linux Support

### Mainline kernel

- **QCS8550 / QCM8550**: [SM8550 matrix](https://linux-msm.github.io/mainline-status/soc/sm8550). Both SKUs are listed there.
- **QCS8250**: [SM8250 matrix](https://linux-msm.github.io/mainline-status/soc/sm8250).
- **SDA845**: [SDM845 matrix](https://linux-msm.github.io/mainline-status/soc/sdm845). SDA845 is listed there.
- **Q-8750**: The [SM8750 matrix](https://linux-msm.github.io/mainline-status/soc/sm8750) tracks the related Oryon platform. The SKU listed there is CQ8750S.
- **QCS8275 / QCS8300**: [Monaco matrix](https://linux-msm.github.io/mainline-status/soc/monaco). Both SKUs are listed there. Untested on 6.18.

### Mesa GPU support

- [x] Adreno 650 and Adreno 630 are supported by [Freedreno](https://docs.mesa3d.org/drivers/freedreno.html)
- [x] The SM8550 GPU is supported by Freedreno

---

## Resources

- [Q8 series](https://www.qualcomm.com/internet-of-things/products/q8-series)
- [IQ8 series](https://www.qualcomm.com/internet-of-things/products/iq8-series)
- [Q-8750 product brief](https://docs.qualcomm.com/doc/87-94329-1/87-94329-1_REV_B_Qualcomm_Dragonwing_Q-8750_Processor_Product_Brief.pdf)
- [IQ8 product brief](https://docs.qualcomm.com/doc/87-83839-1/87-83839-1_REV_A_Qualcomm_IQ8_Series_Product_Brief________.pdf)
- [Qualcomm Introduces Industrial-Grade IQ Series](https://www.qualcomm.com/news/releases/2024/10/qualcomm-introduces-industrial-grade-iq-series-and-iot-solutions)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)

---

## Boards with Dragonwing Q8 / IQ8

List of boards:

{{< taglist tag="QCS8300" style="cards" >}}

{{< taglist tag="QCS8275" style="cards" >}}

{{< taglist tag="Q-8750" style="cards" >}}

{{< taglist tag="QCM8550" style="cards" >}}

{{< taglist tag="QCS8550" style="cards" >}}

{{< taglist tag="QCS8250" style="cards" >}}

{{< taglist tag="SDA845" style="cards" >}}
