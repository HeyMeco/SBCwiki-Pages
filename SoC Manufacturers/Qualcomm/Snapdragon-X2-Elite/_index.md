---
weight: 18
title: Snapdragon X2 Elite
soc-series:
- Snapdragon
soc:
- X2E-96-100
- X2E-94-100
- X2E-90-100
- X2E-88-100
- X2E-84-100
- X2E-80-100
- X2E-78-100
tags:
- SOC-Qualcomm
- Snapdragon
summary: Qualcomm Snapdragon X2 Elite PC processors, with 3rd-gen Oryon cores up to 18 cores and 5.0 GHz, Adreno X2 GPUs, and up to 85 TOPS.
---
# Snapdragon X2 Elite

The Qualcomm Snapdragon X2 Elite is the second Snapdragon X Elite generation. The CPU is Qualcomm's 3rd-gen Oryon, on a 3 nm process. X2E-96-100 is sold as Snapdragon X2 Elite Extreme. The previous generation is [Snapdragon X Elite](/docs/soc-manufacturers/qualcomm/snapdragon-x-elite/).

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

Where Qualcomm publishes the cluster split, the 18-core parts are 12 prime cores and 6 performance cores, and the 12-core parts are 6 prime cores and 6 performance cores. X2E-94-100 and X2E-90-100 are listed by core count and maximum clock.

Shared features on the published briefs: Adreno DPU with eDP 1.5 up to 4K144, DisplayPort 1.4 for three displays up to 4K144 or 5K60, NVMe on PCIe Gen 5, and UFS 4.0. Adreno VPU decode covers AV1, H.265, and H.264, up to dual 8K60 on the higher parts. The Hexagon NPU is paired with dual micro NPUs on the Sensing Hub. Configured memory capacity is device-specific, up to 128 GB, and up to 128 GB or more on X2E-96-100.

### Also known as

- Glymur
- Snapdragon X2 Elite Extreme (X2E-96-100)

---

## Linux Support

### Mainline kernel

- [ ] No mainline status matrix lists the X2 Elite SKUs yet
- Qualcomm's [Linux on Snapdragon X2 early developer preview](https://www.qualcomm.com/developer/blog/2026/09/announcing-linux-on-snapdragon-x2-series-early-developer-preview) is the vendor starting point

## Windows on Arm Support

- Windows on Arm is the shipping OS for these processors. Boot support depends on the board vendor.

---

## Resources

- [Snapdragon X series](https://www.qualcomm.com/laptops/products)
- [Snapdragon X2 Elite product brief](https://www.qualcomm.com/content/dam/qcomm-martech/dm-assets/documents/Snapdragon-X2-Elite-Product-Brief.pdf)

---

## Boards with Snapdragon X2 Elite

List of boards:

{{< taglist tag="X2E-96-100" style="cards" >}}

{{< taglist tag="X2E-94-100" style="cards" >}}

{{< taglist tag="X2E-90-100" style="cards" >}}

{{< taglist tag="X2E-88-100" style="cards" >}}

{{< taglist tag="X2E-84-100" style="cards" >}}

{{< taglist tag="X2E-80-100" style="cards" >}}

{{< taglist tag="X2E-78-100" style="cards" >}}
