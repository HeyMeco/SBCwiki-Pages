---
weight: 14
title: Dragonwing Q5 Series
soc-series:
- Dragonwing
soc:
- QCS5430
- QCM5430
- QRB5165
tags:
- SOC-Qualcomm
- Dragonwing-Q
summary: Qualcomm Dragonwing Q5 processors QCS5430, QCM5430, and QRB5165 for handhelds, cameras, kiosks, and robots.
---
# Dragonwing Q5 Series

The Qualcomm Dragonwing Q5 series covers rugged handhelds, scanners, cameras, kiosks, and mobile robots. QCS5430 and QCM5430 are lower Cortex-A78 parts on the same platform as [QCS6490](/docs/soc-manufacturers/qualcomm/dragonwing-6490/). QRB5165 is a robotics Cortex-A77 part.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

### Variant Differences:

- **QCS5430**: Wi-Fi 6 and Wi-Fi 6E, 1x1, Bluetooth 5.2. Android, Linux, Ubuntu, and Windows. Two displays, DisplayPort 1.4, one 4-lane DSI, and two PCIe lanes. 10-year longevity. CPU, GPU, camera, and AI are sold as feature packs.
- **QCM5430**: All four Cortex-A78 cores are enabled, rather than the 6-core mix on QCS5430. Wi-Fi 6E 2x2, and the same OS list. The modem prefix is the other difference from QCS5430.
- **QRB5165**: Spectra 480 ISP, with 200 MP photos, 8K recording, and 4K HDR. Wi-Fi 6, Wi-Fi 5, and Wi-Fi 4 at 2x2, Bluetooth 5.1. Linux and Ubuntu. Three displays. 11-year longevity.

---

## Linux Support

### Mainline kernel

- **QCS5430 / QCM5430**: Listed on the [Kodiak matrix](https://linux-msm.github.io/mainline-status/soc/kodiak), with QCS6490.
- **QRB5165**: Listed on the [SM8250 matrix](https://linux-msm.github.io/mainline-status/soc/sm8250).

### Mesa GPU support

- [x] Adreno 643 and Adreno 650 are supported by [Freedreno](https://docs.mesa3d.org/drivers/freedreno.html)

---

## Resources

- [Q5 series](https://www.qualcomm.com/internet-of-things/products/q5-series)
- [QCS5430 / QCM5430 product brief](https://docs.qualcomm.com/bundle/publicresource/87-43681-1_REV_C_Qualcomm_QCS5430_QCM5430_Processors_Product_Brief.pdf)
- [QRB5165 product brief](https://docs.qualcomm.com/doc/87-28730-1/87-28730-1_REV_D_Qualcomm_Dragonwing_QRB5165_Processor_Product_Brief.pdf)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)

---

## Boards with Dragonwing Q5

List of boards:

{{< taglist tag="QCS5430" style="cards" >}}

{{< taglist tag="QCM5430" style="cards" >}}

{{< taglist tag="QRB5165" style="cards" >}}
