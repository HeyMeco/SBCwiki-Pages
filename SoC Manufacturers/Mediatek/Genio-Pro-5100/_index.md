---
weight: 0
title: Genio Pro 5100 / Kompanio Ultra 910
soc-series:
- Genio
soc:
- Genio-Pro-5100
- Kompanio-Ultra-910
- MT8894
- MT8196
tags:
- SOC-MTK
summary: MediaTek Genio Pro 5100 (MT8894) and Kompanio Ultra 910 (MT8196). Same Dimensity 9400-class silicon — IoT and Chromebook grades with 1x X925 + 3x X4 + 4x A720, Immortalis-G925 MC11, and 50+ TOPS NPU.
---
# Genio Pro 5100 / Kompanio Ultra 910

The MediaTek Genio Pro 5100 and Kompanio Ultra 910 are the IoT and Chromebook grades of the same Dimensity 9400-class SoC on TSMC 3 nm. Genio Pro 5100 is the embedded part (MT8894). Kompanio Ultra 910 is the Chromebook part (MT8196). Both use an all-big-core Arm v9.2 cluster, an Immortalis-G925 MC11 GPU, and MediaTek's 8th-generation NPU.

## General Specifications
{{% details title="Specs" open=true %}}

| **Part** | **CPU** | **GPU** | **Memory** | **AI** |
|----------|---------|---------|------------|--------|
| **Genio Pro 5100 / MT8894** | Industrial: 1x Cortex-X925 @ 3.1 GHz<br>3x Cortex-X4 @ 2.8 GHz<br>4x Cortex-A720 @ 2.3 GHz<br>3 nm | Immortalis-G925 MC11 @ 1.1 GHz<br>3.1 TFLOPs | x64 LPDDR5X-8533<br>Up to 30 GB | 8th-gen NPU, 53 TOPS<br>(4x MDLA5.5 + 2x MVPU) |
| **Kompanio Ultra 910 / MT8196** | 1x Cortex-X925 up to 3.62 GHz<br>3x Cortex-X4<br>4x Cortex-A720<br>12 MB L3 + 10 MB SLC<br>3 nm | Immortalis-G925 MC11 | LPDDR5X up to 8533 Mbps | MediaTek NPU 890<br>Same GenAI-class NPU as Genio Pro 5100 |

{{% /details %}}

### Also known as

- MT8894 (Genio Pro 5100)
- MT8196 (Kompanio Ultra 910)
- Dimensity 9400-class (no phone 5G modem)

### Variant Differences:

- **Genio Pro 5100**: Industrial IoT grade. Longevity until 2036. Tj −40°C to 105°C. UFS 4.1, dual 2.5 GbE with TSN, PCIe 4.0, triple 4K60 display, up to 16 camera virtual channels, 8K30 encode/decode. Dual HiFi 5 audio DSPs. Yocto, Debian, Ubuntu, and ROS. Aimed at AMRs, drones, edge AI, transportation, and logistics.
- **Kompanio Ultra 910**: Chromebook grade. Higher peak X925 clock (up to 3.62 GHz). UFS 4.0. Internal 4K60 plus up to two 4K external displays. Wi-Fi 7 and Bluetooth 6.0 on the platform. ChromeOS is the primary OS. MediaTek notes that agentic AI, Bluetooth 6.0, and ray tracing are not supported on ChromeOS even when the silicon has those blocks.

---

## Linux Support

### Mainline kernel

- [ ] Fully supported
- [x] Works but not all features are implemented

Collabora tracks mainline bring-up for MT8196 Chromebook platforms. Kernel work for shared blocks (for example the MT8196 DSI PHY) also covers Genio Pro 5100 (MT8894).

---

## Resources

- [Genio Pro 5100](https://genio.mediatek.com/genio-pro-5100)
- [Genio Pro 5100 factsheet (PDF)](https://www.mediatek.com/hubfs/MediaTek%20Assets/Pdfs/FactSheet%20Assets/Pdf/Factsheet_Genio-5100.pdf)
- [Kompanio Ultra 910](https://www.mediatek.com/products/laptops-and-tablets/kompanio/mediatek-kompanio-ultra)
- [Collabora MT8196 mainline status](https://gitlab.collabora.com/mediatek/aiot/wiki/-/blob/main/mainline-status-8196.md)

---

## Boards with Genio Pro 5100 / Kompanio Ultra 910

List of boards:

{{< taglist tag="Genio-Pro-5100" style="cards" >}}

{{< taglist tag="Kompanio-Ultra-910" style="cards" >}}

{{< taglist tag="MT8894" style="cards" >}}

{{< taglist tag="MT8196" style="cards" >}}
