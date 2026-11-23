---
weight: 10
title: Dragonwing Q8 / IQ8
bookCollapseSection: true
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
summary: "Qualcomm Dragonwing Q8 / IQ8 specs: Q-8750 (Oryon CPU, up to 77 TOPS), QCS8550 / QCM8550, QCS8250 and SDA845, plus the industrial IQ8 Monaco parts QCS8275 and QCS8300 (up to 40 dense TOPS). Boards and Linux support."
seeAlso:
- /news/articles/arduino-ventuno-q-first-look-ew26
- /docs/soc-manufacturers/cix/cd8180-p1
- /docs/soc-manufacturers/rockchip/rk3688
---
# Dragonwing Q8 / IQ8

The Qualcomm Dragonwing Q8 series is the top of the commercial Q family. Qualcomm rates it at up to 77 TOPS, for smart displays, video conferencing, wearables, body and motion cameras, and set-top boxes. IQ8 is the industrial series, codename Monaco, for fleet cameras, machine vision, gateways, PLCs, and robotics. These parts do not share one CPU. Q-8750 uses Qualcomm's custom Oryon cores. QCS8550 and QCM8550 are the SM8550 cluster. QCS8250 and SDA845 are older Cortex-A77 and Cortex-A75 designs. QCS8275 and QCS8300 use Cortex-A78C and Cortex-A55 cores, which Qualcomm sells as Kryo Gen 6.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

### Chips

Each chip has its own page with full specifications, Linux support, and boards.

- [**Q-8750**](./q-8750/): Oryon Gen 2 CPU and up to 77 TOPS, the top of the commercial Q8 series.
- [**QCS8550 / QCM8550**](./qcs8550/): The SM8550 cluster. QCM8550 adds a Snapdragon X70 5G modem.
- [**QCS8275 / QCS8300**](./qcs8275/): The industrial IQ8 SoC, codename Monaco. QCS8300 adds a safety island.
- [**QCS8250**](./qcs8250/): Cortex-A77 SoC with Adreno 650, 15-year longevity.
- [**SDA845**](./sda845/): The IoT SKU of SDM845.

---

## Linux Support

Mainline kernel and Mesa status differ per chip. See each chip page above.

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

{{< taglist tag="Q-8750" style="cards" >}}

{{< taglist tag="QCS8550" style="cards" >}}

{{< taglist tag="QCM8550" style="cards" >}}

{{< taglist tag="QCS8300" style="cards" >}}

{{< taglist tag="QCS8275" style="cards" >}}

{{< taglist tag="QCS8250" style="cards" >}}

{{< taglist tag="SDA845" style="cards" >}}
