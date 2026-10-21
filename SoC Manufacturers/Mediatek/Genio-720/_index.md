---
weight: 2
title: Genio 720 / 520 / Kompanio 540
soc-series:
- Genio
- Kompanio
soc:
- Genio-720
- Genio-520
- Kompanio-540
- MT8391
- MT8371
- MT8189
tags:
- SOC-MTK
- Kompanio
aliases:
- /docs/soc-manufacturers/mediatek/genio-520/
- /docs/soc-manufacturers/mediatek/kompanio-540/
summary: MediaTek Genio 720 (MT8391), Genio 520 (MT8371), and Kompanio 540 (MT8189). Shared 2x A78 + 6x A55 cluster on 6 nm, with up to 10 TOPS platform AI on the Genio parts.
---
# Genio 720 / 520 / Kompanio 540

These three names share the same CPU layout: two Cortex-A78 cores and six Cortex-A55 cores on 6 nm. **Genio 720** and **Genio 520** are pin-compatible IoT parts with an 8th-generation MediaTek NPU and optional Wi-Fi 6/6E baseband. **Kompanio 540** is the Chromebook SKU under the MT8189 part number, aimed at entry Chromebooks rather than industrial IoT.

## General Specifications
{{% details title="Specs" open=true %}}

| **Part** | **CPU** | **GPU** | **Memory** | **AI** |
|----------|---------|---------|------------|--------|
| **Genio 720 / MT8391** | Consumer: 2x A78 @ 2.6 GHz + 6x A55 @ 2.0 GHz<br>Industrial: 2x A78 @ 2.4 GHz + 6x A55 @ 2.0 GHz<br>6 nm | Mali-G57 MC2 @ 1.1 GHz | x32 LPDDR4X-4266 up to 8 GB<br>x32 LPDDR5(X)-6400 up to 16 GB | 8th-gen NPU, 9 TOPS (MDLA5.3)<br>Up to 10 TOPS platform AI |
| **Genio 520 / MT8371** | Consumer: 2x A78 @ 2.2 GHz + 6x A55 @ 2.0 GHz<br>Industrial: 2x A78 @ 2.0 GHz + 6x A55 @ 1.8 GHz<br>6 nm | Mali-G57 MC2 @ 880 MHz | Same LPDDR4X / LPDDR5(X) options as Genio 720 | Same 8th-gen NPU class as Genio 720 |
| **Kompanio 540 / MT8189** | 2x A78 @ 2.6 GHz + 6x A55 @ 2.0 GHz<br>6 nm | Mali-G57 MC2 | LPDDR5 up to 6400 Mbps<br>LPDDR4X up to 4266 Mbps | Chromebook SKU; no separate Genio NPU rating published |

{{% /details %}}

### Variant Differences:

- **Genio 720**: Dual ISP (32 MP or 16+16 MP at 30 fps). Dual 2.5K60 or single UW5K60 / 4K60 display. Video decode H.264/H.265/VP9 at 4K60, encode H.264/H.265 at 4K30. UFS 3.1, eMMC 5.1. Integrated Wi-Fi 6 1x1 or Wi-Fi 6E 2x2 with Bluetooth 5.3. Longevity until 2035. Package 13.8 × 11.8 mm.
- **Genio 520**: Pin- and software-compatible with Genio 720. One ISP (16 MP at 30 fps). Lower CPU and GPU clocks. Same display, storage, I/O, and temperature grades. OSM reference design available.
- **Kompanio 540**: Chromebook branding. UFS 3.1 or eMMC 5.1. Internal display up to 2.5K; external up to 4K60 via DP (MediaTek says 4K60 external is not used on Kompanio 540 Chromebooks). Video decode 4K60, encode FHD60. Pairs with Filogic Wi-Fi 7 and Bluetooth 6.0 on the platform. Aimed at education and everyday Chromebooks.

Shared Genio I/O includes USB 2.0/3.2, GbE with TSN, PCIe 2.0, MIPI-DSI / eDP / DP, and consumer (−20°C to 95°C Tj) or industrial (−40°C to 105°C Tj) grades. OS support on Genio is Android, IoT Yocto, and Ubuntu.

---

## Linux Support

### Mainline kernel

- **Genio 520 / Genio 720**: Mainline boots. MediaTek states many drivers are upstreamed; stateful video, ISP, NPU, and GPU remain proprietary or third-party. Panfrost covers the Mali-G57 GPU in Mesa.
- **Kompanio 540 / MT8189**: Chromebook bring-up follows MediaTek's Kompanio ChromeOS stack; mainline coverage depends on the specific board.

---

## Resources

- [Genio 720](https://genio.mediatek.com/genio-720)
- [Genio 520](https://genio.mediatek.com/genio-520)
- [Kompanio 540](https://www.mediatek.com/products/laptops-and-tablets/kompanio/mediatek-kompanio-540)
- [Genio IoT portfolio](https://www.mediatek.com/products/iot/genio-iot)

---

## Boards with Genio 720 / 520 / Kompanio 540

List of boards:

{{< taglist tag="Genio-720" style="cards" >}}

{{< taglist tag="Genio-520" style="cards" >}}

{{< taglist tag="Kompanio-540" style="cards" >}}
