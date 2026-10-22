---
weight: 1
title: Rockchip RK3668
bookHidden: true
#bookCollapseSection: true
soc-series:
- RK36XX
soc:
- RK3668
tags: 
- SOC-RK-Upcoming
summary: Upcoming Rockchip RK3668 6nm SoC — octa-core Armv9.2 (6× Cortex-A725 + 2× A520), Mali-G2 Pro MC4 (1.23 TFLOPS), 44 TOPS sparse NPU, LPDDR5X/LPDDR6. Engineering samples Q1 2027.
---
# Rockchip RK3668

> **Status:** Developing. Rockchip’s [application brief REL02](https://dl.radxa.com/rock6/6b/RK3668-SoC-Application-REL02-20261009.pdf) (9 October 2026) targets **engineering samples in Q1 2027**. Clocks and the comparison figures below are Rockchip’s estimates from that brief.

RK3668 is the **6 nm** SoC on Rockchip’s flagship roadmap, above **RK3588**. **RK3688** is still the planned flagship above it. The brief specifies an octa-core **Armv9.2** CPU, a **Mali-G2 Pro MC4** GPU, and a **44 TOPS** sparse NPU.

The 2025 RKDC notes (10× Armv9.3 Cortex-A730/A530, Magni GPU, 16 TOPS, Q4 2026) are an earlier aggregation. This page follows the [October 2026 brief](https://dl.radxa.com/rock6/6b/RK3668-SoC-Application-REL02-20261009.pdf).

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

Rockchip lists target applications as Android servers, interactive large-format displays, NVR, CVR, display control, robotics, NAS, PLC, cockpit, and box PCs.

---

## Rockchip comparison charts

Figures are from the [October 2026 brief](https://dl.radxa.com/rock6/6b/RK3668-SoC-Application-REL02-20261009.pdf). They are Rockchip’s projections for RK3668 (and Rockchip’s own numbers for the other SoCs), so they will not match independent Geekbench runs such as the [RK3572 EVB results](/news/articles/exclusive-rk3572-benchmarked-at-ew26/).

Rockchip states a per-core DMIPS ratio of A725/A76 = **1.51**, and a Geekbench 6 single-core ratio of A725/A76 = **1.40**. Multi-core DMIPS on the chart is a linear sum across cores.

| | RK3668 | RK3588 | RK3576 | RK3572 | RK3568B2 |
|--|--------|--------|--------|--------|----------|
| CPU (kDMIPS) | 213.8 | 105.0 | 76.6 | 61.2 | 27.6 |
| Geekbench 6 single-core | 1340 | 900 | 377 | 380 | 296 |
| GPU FP32 (GFLOPS) | 1228 | 512 | 129 | 67 | 38 |
| GFXBench Manhattan 3.0 1080p offscreen (fps) | 287.0 | 144.4 | 35.4 | 20.1 | 10.5 |
| NPU (TOPS, INT8 sparse) | 44.0 | 6.0 | 6.0 | 4.2 | 1.0 |
| Peak DRAM (GB/s) | 128.0 | 44.0 | 22.0 | 22.0 | 12.8 |
| Peak flash (GB/s) | 11.7 | 0.4 | 2.9 | 2.9 | 0.4 |

---

## Linux Support

No public BSP or mainline support yet. Engineering samples are scheduled for Q1 2027.

---

## Documentation

- [RK3668 SoC Application brief, REL02 (9 October 2026)](https://dl.radxa.com/rock6/6b/RK3668-SoC-Application-REL02-20261009.pdf) — hosted on Radxa’s Rock 6B download server

---

## Further reading

- [State of Embedded: Q4 2025 Overview](/news/articles/state-of-embedded-q4-25/) — RKDC 2025 aggregation (superseded by the October 2026 brief)
- [Exclusive: RK3572 First look & Geekbench results](/news/articles/exclusive-rk3572-benchmarked-at-ew26/) — earlier Q4 2026 outlook for RK3668

---

## Boards with RK3668

No boards announced yet.

{{< taglist tag="RK3668" style="cards" >}}
