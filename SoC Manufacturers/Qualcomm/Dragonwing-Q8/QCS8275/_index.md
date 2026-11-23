---
weight: 3
title: QCS8275 / QCS8300
soc-series:
- Dragonwing
soc:
- QCS8275
- QCS8300
tags:
- SOC-Qualcomm
- Dragonwing-IQ
summary: "Qualcomm Dragonwing IQ8 (QCS8275 / QCS8300, Monaco) specs: Cortex-A78C and Cortex-A55 CPU, Adreno 623 GPU, up to 40 dense TOPS, LPDDR5 with inline ECC, -40°C to 125°C. Linux support and boards."
---
# QCS8275 / QCS8300

Part of the [Dragonwing Q8 / IQ8](/docs/soc-manufacturers/qualcomm/dragonwing-q8/) series. QCS8275 and QCS8300 are the industrial Dragonwing IQ8 SoC, codename Monaco, also sold as IQ-8275 and IQ-8300. Qualcomm targets fleet cameras, machine vision, gateways, PLCs, and robotics. The CPU uses Cortex-A78C and Cortex-A55 cores, which Qualcomm sells as Kryo Gen 6.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

### Details

- **QCS8275**: Industrial grade. AI performance scales from 20 to 40 dense TOPS. Decode is 4K135 for AV1, H.265, H.264, and VP9. Encode is 4K85 for H.264 and H.265. 4x CAN FD and 1x GbE. Yocto Linux and Ubuntu. Rated -40°C to 125°C, supported until 2038.
- **QCS8300**: Same Monaco SoC as QCS8275, with a safety island and planned SIL3 support. AI performance is 40 dense TOPS.

### Also known as

- IQ-8275
- IQ-8300
- Monaco

---

## Linux Support

### Mainline kernel

- [Monaco matrix](https://linux-msm.github.io/mainline-status/soc/monaco). Both SKUs are listed there. Untested on 6.18.

### Mesa GPU support

- Adreno 623 is an a6xx_gen4 GPU. See [Adreno GPUs](/docs/soc-manufacturers/qualcomm/adreno-gpu/) for the [Freedreno](https://docs.mesa3d.org/drivers/freedreno.html) generation.

---

## Resources

- [IQ8 series](https://www.qualcomm.com/internet-of-things/products/iq8-series)
- [IQ8 product brief](https://docs.qualcomm.com/doc/87-83839-1/87-83839-1_REV_A_Qualcomm_IQ8_Series_Product_Brief________.pdf)
- [Qualcomm Introduces Industrial-Grade IQ Series](https://www.qualcomm.com/news/releases/2024/10/qualcomm-introduces-industrial-grade-iq-series-and-iot-solutions)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)

---

## Boards with QCS8275 / QCS8300

List of boards:

{{< taglist tag="QCS8300" style="cards" >}}

{{< taglist tag="QCS8275" style="cards" >}}
