---
weight: 5
title: Rockchip RK3572
#bookCollapseSection: true
soc-series:
- RK35XX
soc:
- RK3572
tags: 
- SOC-RK
summary: Rockchip RK3572 mid-range 8nm AIoT processor — octa-core hybrid (2× Cortex-A73 + 6× A53), Mali-G310 GPU, 4 TOPS sparse NPU, 8K video decode.
---
# Rockchip RK3572

Rockchip [officially launched](https://www.rock-chips.com/a/cn/news/rockchip/2026/0508/2168.html) the RK3572 on 8 May 2026 as its mid-range **8nm** AIoT platform. It sits in the same class as **RK3568** and **RK3576**, with a newer DRAM controller, UFS, and VPU, and is the first non-flagship Rockchip part with a **Mali v10 (CSF)** GPU — **Mali-G310 v2** — which benefits from upstream **Panthor** and **Tyr** work in Mesa.

Rockchip positions it as doubling performance and cutting typical-scene power by more than 50% versus the previous mid-range generation, with AnTuTu v10 scores above **310,000** on a tablet configuration.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **Rockchip RK3572** |
|---------|---------------------|
| **Process** | 8nm |
| **CPU** | Octa-core hybrid: <br> 2× ARM Cortex-A73 <br> 6× ARM Cortex-A53 <br> Up to 2.2 GHz (module spec; datasheet clocks TBD) |
| **RAM** | 32-bit LPDDR4/LPDDR4X-4266 · LPDDR5/LPDDR5X-5500 <br> Up to 4 ranks, 16 GB addressing |
| **Storage** | UFS 2.0 (2-lane, HS-G3) · eMMC 5.1 (HS400) · SD 3.0 / MMC 4.51 · FSPI |
| **GPU** | Mali-G310 v2 MC1 <br> OpenGL® ES 1.1/2.0/3.2, OpenCL™ 3.0, Vulkan® 1.4 |
| **NPU** | 4 TOPS sparse INT8 <br> INT4/INT8/INT16/FP4/FP8/FP16/BF16, W4A16 asymmetric MAC |
| **VPU** | H.265/VP9/AV1/AVS2 decode up to 8K@30fps or 4K@120fps <br> H.264 decode up to 4K@60fps <br> H.264/H.265 encode up to 4K@40fps |
| **Display** | Dual independent display: 4K@60fps + 2K@60fps <br> HDMI 2.1, eDP 1.3, MIPI DSI 1.2, parallel RGB/BT.656/BT.1120, E-ink |
| **ISP** | 12 MP ISP · up to 5 camera inputs <br> 2× MIPI CSI-2 D-PHY (each 4-lane or 2×2-lane) + DVP |
| **Connectivity** | PCIe 2.1 · SATA 3.1 · USB DRD 3.0/2.0 · dual Gigabit Ethernet <br> SDIO 3.0 · DSMC · CAN, I2C, I3C, SPI, UART |
| **Package** | FCCSP550L (14.3 × 15.5 mm) |

{{% /details %}}
<br>
{{% details title="Block Diagram" open=false %}}

![RK3572 Block Diagram](images/RK3572-Block-Diagram.png?f=webp)

{{% /details %}}

Rockchip’s published power figures (tablet, 8 GB LPDDR5 + 128 GB UFS, display/touch removed, Wi-Fi/BT off): deep standby below **10 mW**, 1080p playback **670 mW**, light 3D GPU load below **1 W**. Most real-world minimum-system scenes are claimed under 1 W.

---

## Linux Support

Forlinx provides a customer-delivered Linux 6.12 BSP for the OK3572-C (Forlinx Desktop 24.04, Debian 13, and Android 16). The [June 2026 announcement](https://www.cnx-software.com/2026/06/04/forlinx-launches-rockchip-rk3572-system-on-module-som-and-development-board-with-linux-6-12-bsp/) marked those images as R&D. [Firefly’s ICORE-3572Q38](https://www.t-firefly.com/products/icore-3572q38) lists Debian and Ubuntu. No mainline support is documented yet. The Mali-G310 v2 is a CSF GPU, so Panthor/Tyr support from RK3588 should apply as boards reach upstream. The [EW26 EVB](https://sbcwiki.com/news/articles/exclusive-rk3572-benchmarked-at-ew26/) ran pre-release software.

---

## Benchmarks (pre-release EVB)

Geekbench 6 results from the Embedded World 2026 evaluation board running **pre-release software** — figures may improve on retail boards. That EVB was described as hexa-core; official silicon is octa-core (2× A73 + 6× A53).

| Benchmark | RK3572 | RK3568 | RK3576 | RK3588 |
|-----------|--------|--------|--------|--------|
| Single-core | 332 | 225 | 319 | 813 |
| Multi-core | 1158 | 571 | 1332 | 2944 |
| Vulkan (GPU) | 838 | — | — | 3637 |

Thermals on the show floor were notably mild — the package stayed warm rather than hot under sustained load, unlike typical RK3588 behaviour.

---

## Documentation
- [Official RK3572 announcement (Rockchip, 8 May 2026)](https://www.rock-chips.com/a/cn/news/rockchip/2026/0508/2168.html)
- [RK3572 Datasheet V1.1](https://rockchip.fr/RK3572%20datasheet%20V1.1.pdf)
- Technical Reference Manual

---

## Further reading

- [Exclusive: RK3572 First look & Geekbench results](https://sbcwiki.com/news/articles/exclusive-rk3572-benchmarked-at-ew26/) — hands-on benchmarks from the EW26 EVB
- [State of Embedded: Q4 2025 Overview](https://sbcwiki.com/news/articles/state-of-embedded-q4-25/) — RKDC roadmap (pre-launch aggregated specs)

---

## Boards with RK3572

- [Firefly ICORE-3572Q38](https://www.t-firefly.com/products/icore-3572q38) — 38 × 38 mm SoM
- [Forlinx FET3572-C SoM and OK3572-C development board](https://www.forlinx.net/industrial-news/forlinx-fet3572-c-som-rockchip-rk3572-828.html) — Linux 6.12 BSP

{{< taglist tag="RK3572" style="cards" >}}
