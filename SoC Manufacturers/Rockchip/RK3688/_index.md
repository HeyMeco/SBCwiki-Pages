---
weight: 0
title: Rockchip RK3688
bookHidden: true
#bookCollapseSection: true
soc-series:
- RK36XX
soc:
- RK3688
tags: 
- SOC-RK-Upcoming
summary: Upcoming Rockchip RK3688 flagship — 12-core Armv9.3 CPU (4–5nm), Arm Magni GPU (2+ TFLOPS), 32 TOPS NPU, 8-channel LPDDR5/5x/6, UFS 4.0. Expected Q1 2027.
---
# Rockchip RK3688

> **Status:** Upcoming — Rockchip roadmap targets **Q1 2027**. Specifications below are aggregated from the [Rockchip Developer Conference (RKDC)](https://sbcwiki.com/news/articles/state-of-embedded-q4-25/) and may change before release.

Rockchip's next-generation flagship SoC, positioned above the RK3588. RK3688 is expected to use Arm's new **Magni** GPU generation (marketed as [Arm Mali G1 Ultra](/docs/soc-manufacturers/arm/mali-gpu/)) and the **RKNN-P3** NPU block.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **Rockchip RK3688** |
|---------|---------------------|
| **Process** | 4–5 nm (300K+ DMIPS) |
| **CPU** | 12-core: 8× Cortex-A730 + 4× Cortex-A530 |
| **RAM** | 8-channel LPDDR5 / LPDDR5x / LPDDR6 (up to 200 GB/s) |
| **GPU** | Arm Mali Magni (2+ TFLOPS) |
| **NPU** | 32 TOPS (RKNN-P3) |
| **Storage** | UFS 4.0 |
| **VPU** | 16K@30fps decoder · 8K@60fps encoder |

{{% /details %}}

---

## Linux Support

Not yet available — no public BSP or mainline support at this stage.

---

## Further reading

- [State of Embedded: Q4 2025 Overview](https://sbcwiki.com/news/articles/state-of-embedded-q4-25/) — RKDC roadmap and aggregated specs
- [Exclusive: RK3572 First look & Geekbench results](https://sbcwiki.com/news/articles/exclusive-rk3572-benchmarked-at-ew26/) — RK3572 EVB at Embedded World 2026; RK3688 outlook (Q1 2027)

---

## Boards with RK3688

No boards announced yet.

{{< taglist tag="RK3688" style="cards" >}}
