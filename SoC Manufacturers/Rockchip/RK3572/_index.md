---
weight: 5
title: Rockchip RK3572
bookHidden: true
#bookCollapseSection: true
soc-series:
- RK35XX
soc:
- RK3572
tags: 
- SOC-RK-Upcoming
summary: Upcoming Rockchip RK3572 — hexa-core (2× A73 + 4× A53), Mali-G310 v2 GPU with upstream Panthor support, 3 TOPS NPU, 4K@120fps decode. Expected Q3 2026.
---
# Rockchip RK3572

> **Status:** Upcoming — Rockchip roadmap targets **Q3 2026**. First public EVB shown at [Embedded World 2026](https://sbcwiki.com/news/articles/exclusive-rk3572-benchmarked-at-ew26/); expected in Zero-sized SBCs and similar mid-range boards.

Interim SoC in the same class as **RK3568** and **RK3576**, but with Rockchip's latest DRAM controller, UFS, and VPU IP. First non-flagship Rockchip part with a **Mali v10 (CSF)** GPU — **Mali-G310 v2** — which benefits from upstream **Panthor** and **Tyr** work in Mesa and the mainline kernel.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **Rockchip RK3572** |
|---------|---------------------|
| **CPU** | Hexa-core: 2× Cortex-A73 @ 2.3 GHz + 4× Cortex-A53 @ 2.0 GHz |
| **RAM** | 32-bit LPDDR4 / LPDDR4x · LPDDR5 / LPDDR5x |
| **Storage** | UFS 2.1 · eMMC |
| **GPU** | Arm Mali-G310 v2 (OpenGL ES / Vulkan / OpenCL) |
| **NPU** | 3 TOPS |
| **VPU** | 4K@120fps decoder · 4K@30fps encoder |

{{% /details %}}

---

## Benchmarks (pre-release EVB)

Geekbench 6 results from the Embedded World 2026 evaluation board running **pre-release software** — figures may improve before retail boards ship.

| Benchmark | RK3572 | RK3568 | RK3576 | RK3588 |
|-----------|--------|--------|--------|--------|
| Single-core | 332 | 225 | 319 | 813 |
| Multi-core | 1158 | 571 | 1332 | 2944 |
| Vulkan (GPU) | 838 | — | — | 3637 |

Thermals on the show floor were notably mild — the package stayed warm rather than hot under sustained load, unlike typical RK3588 behaviour.

---

## Linux Support

Not yet available in vendor BSPs or mainline — EVB was running pre-release software at EW26.

---

## Further reading

- [Exclusive: RK3572 First look & Geekbench results](https://sbcwiki.com/news/articles/exclusive-rk3572-benchmarked-at-ew26/) — hands-on benchmarks and roadmap context
- [State of Embedded: Q4 2025 Overview](https://sbcwiki.com/news/articles/state-of-embedded-q4-25/) — RKDC roadmap (initial aggregated specs)

---

## Boards with RK3572

No retail boards announced yet — expected in Zero-sized form factors from Q3 2026.

{{< taglist tag="RK3572" style="cards" >}}
