---
weight: 2
title: QCS8550 / QCM8550
soc-series:
- Dragonwing
soc:
- QCS8550
- QCM8550
tags:
- SOC-Qualcomm
- Dragonwing-Q
summary: "Qualcomm QCS8550 / QCM8550 specs: 4 nm SM8550 with Cortex-X3, A715, A710 and A510 cores, Adreno 740 GPU, LPDDR5X-8400, Wi-Fi 7. QCM8550 adds an X70 5G modem. Linux support and boards."
---
# QCS8550 / QCM8550

Part of the [Dragonwing Q8 / IQ8](/docs/soc-manufacturers/qualcomm/dragonwing-q8/) series. QCS8550 and QCM8550 share the SM8550 application processor.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

### Details

- **QCM8550**: Adds a Snapdragon X70 5G modem. Android, Linux, and Ubuntu. Wi-Fi 7 2x2 and Bluetooth 5.3. Four displays. 10-year longevity.
- **QCS8550**: The standalone version of that processor, without the X70 modem.

### Also known as

- SM8550

---

## Linux Support

### Mainline kernel

- [SM8550 matrix](https://linux-msm.github.io/mainline-status/soc/sm8550). Both SKUs are listed there.

### Mesa GPU support

- [x] The SM8550 GPU (Adreno 740) is supported by [Freedreno](https://docs.mesa3d.org/drivers/freedreno.html)

---

## Resources

- [Q8 series](https://www.qualcomm.com/internet-of-things/products/q8-series)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)

---

## Boards with QCS8550 / QCM8550

List of boards:

{{< taglist tag="QCS8550" style="cards" >}}

{{< taglist tag="QCM8550" style="cards" >}}
