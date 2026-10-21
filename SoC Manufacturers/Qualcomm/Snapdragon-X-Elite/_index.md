---
weight: 19
title: Snapdragon X Elite / IQ-X
soc-series:
- Snapdragon
- Dragonwing
soc:
- X1E-00-1DE
- X1E-84-100
- X1E-80-100
- X1E-78-100
- IQ-X7181
- IQ-X5121
tags:
- SOC-Qualcomm
- Snapdragon
summary: Qualcomm Snapdragon X Elite and Dragonwing IQ-X, one Hamoa SoC. Commercial parts are 12 Oryon cores. IQ-X7181 is the industrial grade of X1E-78-100, and IQ-X5121 is the 8-core industrial part.
---
# Snapdragon X Elite / IQ-X

The Qualcomm Snapdragon X Elite and Dragonwing IQ-X are commercial and industrial grades of the same Hamoa SoC, a 4 nm processor with custom Oryon cores. IQ-X7181 is X1E-78-100 in an industrial package. IQ-X5121 is the 8-core industrial part. The later generation is [Snapdragon X2 Elite](/docs/soc-manufacturers/qualcomm/snapdragon-x2-elite/).

## General Specifications
{{% details title="Specs" open=true %}}

| **Part** | **CPU** | **GPU** | **NPU** | **Memory** |
|----------|---------|---------|---------|------------|
| **X1E-00-1DE** | 12x Oryon<br>3.8 GHz all-core, dual-core boost 4.3 GHz<br>42 MB cache, 4 nm | [Adreno X1-85](/docs/soc-manufacturers/qualcomm/adreno-gpu/#adreno-x-series-pc--compute) @ 1.50 GHz<br>Up to 4.6 TFLOPS | Hexagon<br>45 TOPS | LPDDR5x @ 8448 MT/s<br>8x 16-bit, up to 64 GB<br>135 GB/s |
| **X1E-84-100** | 12x Oryon<br>3.8 GHz all-core, dual-core boost 4.2 GHz<br>42 MB cache, 4 nm | [Adreno X1-85](/docs/soc-manufacturers/qualcomm/adreno-gpu/#adreno-x-series-pc--compute) @ 1.50 GHz<br>Up to 4.6 TFLOPS | Hexagon<br>45 TOPS | LPDDR5x @ 8448 MT/s<br>8x 16-bit, up to 64 GB<br>135 GB/s |
| **X1E-80-100** | 12x Oryon<br>3.4 GHz all-core, dual-core boost 4.0 GHz<br>42 MB cache, 4 nm | [Adreno X1-85](/docs/soc-manufacturers/qualcomm/adreno-gpu/#adreno-x-series-pc--compute) @ 1.25 GHz<br>Up to 3.8 TFLOPS | Hexagon<br>45 TOPS | LPDDR5x @ 8448 MT/s<br>8x 16-bit, up to 64 GB<br>135 GB/s |
| **X1E-78-100** | 12x Oryon @ 3.4 GHz<br>42 MB cache, 4 nm | [Adreno X1-85](/docs/soc-manufacturers/qualcomm/adreno-gpu/#adreno-x-series-pc--compute) @ 1.25 GHz<br>Up to 3.8 TFLOPS | Hexagon<br>45 TOPS | LPDDR5x @ 8448 MT/s<br>8x 16-bit, up to 64 GB<br>135 GB/s |
| **IQ-X7181** | 12x Oryon @ 3.4 GHz<br>Industrial grade of X1E-78-100 | [Adreno](/docs/soc-manufacturers/qualcomm/adreno-gpu/#adreno-x-series-pc--compute) @ 1.25 GHz | Hexagon<br>45 dense TOPS<br>Hexagon V73M | 8x 16-bit LPDDR5x @ 4200 MHz<br>Up to 64 GB |
| **IQ-X5121** | 8x Oryon @ 3.4 GHz<br>Industrial grade | [Adreno](/docs/soc-manufacturers/qualcomm/adreno-gpu/#adreno-x-series-pc--compute) @ 1.1 GHz | Hexagon<br>45 dense TOPS<br>Hexagon V73M | 8x 16-bit LPDDR5x @ 4200 MHz<br>Up to 64 GB |

{{% /details %}}

The commercial parts share an Adreno DPU with eDP 1.4b up to 4K120, and DisplayPort 1.4 for up to three external displays. Adreno VPU decode is 4K120 10-bit for H.264, H.265, VP9, and AV1. Encode is 4K60 10-bit for H.264, H.265, and AV1. Storage is NVMe over PCIe Gen 4, UFS 4.0, and SD 3.0. The Hexagon NPU is paired with dual micro NPUs on the Sensing Hub.

IQ-X adds an industrial package rated -40°C to 105°C, with USB4, 16 PCIe lanes, UFS 4.0, and DisplayPort 1.4a. It supports up to four cameras and up to 2x 5K or 4x 4K displays. The IQ-X series page lists support until 2038. The family comparison lists support until 2036. Target uses are factory automation, HMIs, medical PCs, robotics, panel and box PCs, and smart displays.

### Also known as

- Hamoa
- X1E80100, X1E84100, X1E78100, X1E001DE
- IQ-X7181
- IQ-X5121

---

## Linux Support

### Mainline kernel

- [ ] Fully supported
- [x] Works, but not every feature is implemented. Driver support matrix is [here](https://linux-msm.github.io/mainline-status/soc/hamoa)

### Mesa GPU support

- [x] Adreno X1-85 is supported by [Freedreno](https://docs.mesa3d.org/drivers/freedreno.html) from Mesa 24.2

## Windows on Arm Support

- [Available](https://learn.microsoft.com/en-us/windows-hardware/design/minimum/supported/windows-11-24h2-supported-qualcomm-processors) but depends on the board vendor to provide a compatible bootloader

---

## Resources

- [Snapdragon X series](https://www.qualcomm.com/laptops/products)
- [Snapdragon X Elite product brief](https://docs.qualcomm.com/doc/87-71417-1/87-71417-1_REV_F_Snapdragon_X_Elite_Product_Brief.pdf)
- [IQ-X series](https://www.qualcomm.com/internet-of-things/products/iq-x-series)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)
- [Hamoa mainline status](https://linux-msm.github.io/mainline-status/soc/hamoa)

---

## Boards with Snapdragon X Elite / IQ-X

List of boards:

{{< taglist tag="X1E-00-1DE" style="cards" >}}

{{< taglist tag="X1E-84-100" style="cards" >}}

{{< taglist tag="X1E-80-100" style="cards" >}}

{{< taglist tag="X1E-78-100" style="cards" >}}

{{< taglist tag="IQ-X7181" style="cards" >}}

{{< taglist tag="IQ-X5121" style="cards" >}}
