---
weight: 1
title: Dragonwing Q-8750
soc-series:
- Dragonwing
soc:
- Q-8750
tags:
- SOC-Qualcomm
- Dragonwing-Q
summary: "Qualcomm Dragonwing Q-8750 specs: 8-core Oryon Gen 2 CPU up to 4.32 GHz, Adreno 830 GPU, Hexagon NPU with up to 77 TOPS, LPDDR5X-9600, 8K60 display and decode. Linux support and boards."
---
# Dragonwing Q-8750

Part of the [Dragonwing Q8 / IQ8](/docs/soc-manufacturers/qualcomm/dragonwing-q8/) series. Q-8750 is the top commercial Q8 part, and the only one with Qualcomm's custom Oryon CPU cores.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

### Details

- Android 15+ and Yocto Linux.
- Wi-Fi 7 and Bluetooth 6.0 need companion chips.
- Display outputs are 2x MIPI (up to 8K60) and 8x DisplayPort.
- Video decode goes to 8K60, encode to 8K30.
- Up to 12 cameras with triple 48 MP ISPs.

---

## Linux Support

### Mainline kernel

- The [SM8750 matrix](https://linux-msm.github.io/mainline-status/soc/sm8750) tracks the related Oryon platform. The SKU listed there is CQ8750S.

### Mesa GPU support

- Adreno 830 is an a8xx GPU. See [Adreno GPUs](/docs/soc-manufacturers/qualcomm/adreno-gpu/) for the [Freedreno](https://docs.mesa3d.org/drivers/freedreno.html) generation.

---

## Resources

- [Q8 series](https://www.qualcomm.com/internet-of-things/products/q8-series)
- [Q-8750 product brief](https://docs.qualcomm.com/doc/87-94329-1/87-94329-1_REV_B_Qualcomm_Dragonwing_Q-8750_Processor_Product_Brief.pdf)

---

## Boards with Dragonwing Q-8750

List of boards:

{{< taglist tag="Q-8750" style="cards" >}}
