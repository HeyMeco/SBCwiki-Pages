---
weight: 3
title: Genio 700 / 510
soc-series:
- Genio
soc:
- Genio-700
- Genio-510
- MT8390
- MT8370
tags:
- SOC-MTK
aliases:
- /docs/soc-manufacturers/mediatek/genio-510/
summary: MediaTek Genio 700 (MT8390) and Genio 510 (MT8370). Pin-compatible 6 nm IoT pair with up to 4.0 TOPS NPU, Mali-G57 GPU, and dual 4K display.
---
# Genio 700 / 510

The MediaTek Genio 700 and Genio 510 are a pin-compatible IoT pair on 6 nm. Genio 700 is the higher-compute SKU with an octa-core CPU, Mali-G57 MC3, and a 4.0 TOPS NPU. Genio 510 drops to a hexa-core CPU, Mali-G57 MC2, and 3.2 TOPS. Both target smart retail, home, industrial HMI, signage, and edge vision. Libre Computer and Radxa have shown boards on this family that are not generally available yet.

## General Specifications
{{% details title="Specs" open=true %}}

| **Part** | **CPU** | **GPU** | **Memory** | **AI** |
|----------|---------|---------|------------|--------|
| **Genio 700 / MT8390** | 2x Cortex-A78 @ 2.2 GHz<br>6x Cortex-A55 @ 2.0 GHz<br>6 nm | Mali-G57 MC3 @ 950 MHz | x32 or x64 LPDDR4X-3733<br>Up to 8 GB | 5th-gen NPU, 4.0 TOPS<br>(1x MDLA3.0 + 1x Tensilica VP6) |
| **Genio 510 / MT8370** | 2x Cortex-A78 @ 2.0 GHz<br>4x Cortex-A55 @ 2.0 GHz<br>6 nm | Mali-G57 MC2 @ 950 MHz | Same LPDDR4X options as Genio 700 | 5th-gen NPU, 3.2 TOPS<br>(1x MDLA3.0 + 1x Tensilica VP6) |

{{% /details %}}

### Variant Differences:

- **Genio 700**: Dual ISP (32 MP or 16+16 MP). Dual display up to 4K60+4K30. Decode H.264/H.265/VP9/AV1 at 4K75, encode H.264/H.265 at 4K30. HiFi 5 audio DSP. External Wi-Fi 5 or Wi-Fi 6 combo chips. Longevity until 2034. Package 15 × 15 mm.
- **Genio 510**: Same package and pinout as Genio 700. Dual ISP retained. Decode tops out at 4K60. Lower CPU core count and NPU TOPS. Same USB, GbE with TSN, PCIe 2.0, and consumer / industrial Tj grades (−20°C to 95°C / −40°C to 105°C).

Shared display interfaces include 2x MIPI-DSI, eDP 1.2, DP 1.4, and HDMI 2.0. Storage is eMMC 5.1, SD 3.0, and SPI-NOR. OS support is Android, IoT Yocto, Ubuntu, and AOSP through partners.

---

## Linux Support

### Mainline kernel

- [x] Mainline boots on Genio 510 and Genio 700
- MediaTek states many drivers are upstreamed. Stateful video (VPUD), ISP, NPU, and GPU drivers stay proprietary or third-party. Panfrost covers Mali-G57 in Mesa.

---

## Resources

- [Genio 700](https://genio.mediatek.com/genio-700)
- [Genio 510](https://genio.mediatek.com/genio-510)
- [Genio 700 factsheet (PDF)](https://www.mediatek.com/hubfs/MediaTek%20Assets/Pdfs/FactSheet%20Assets/Pdf/Factsheet%20-%20Genio%20700.pdf)
- [Genio IoT portfolio](https://www.mediatek.com/products/iot/genio-iot)

---

## Boards with Genio 700 / 510

List of boards:

{{< taglist tag="Genio-700" style="cards" >}}

{{< taglist tag="Genio-510" style="cards" >}}
