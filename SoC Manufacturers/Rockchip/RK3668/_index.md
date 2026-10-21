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

| **SoC** | **Rockchip RK3668** |
|---------|---------------------|
| **Process** | 6 nm |
| **CPU** | Octa-core Armv9.2, 64-bit only: <br> 6× ARM Cortex-A725, up to 2.5 GHz (expected) <br> 2× ARM Cortex-A520, up to 2.2 GHz (expected; Rockchip rates A520 in the same class as Cortex-A73) <br> SVE2 · RME, MTE, PAC, BTI |
| **Cache** | 4 MB L3 · 4 MB system-level cache · 4 MB SRAM |
| **RAM** | 64-bit LPDDR5/LPDDR5X-8533 (4×16-bit, 68 GB/s) <br> 96-bit LPDDR6-10667 (4×24-bit, 128 GB/s peak) <br> Up to 64 GB addressing <br> Rockchip derates peak LPDDR6 to about 90 GB/s (128 × 0.88 × 0.8) |
| **Storage** | UFS 4.0, 2-lane, Gear 5B (11.7 GB/s) <br> eMMC 5.1 (HS400) · SDIO 3.0 (HS200) · SDMMC · NVMe · SFC · SPI |
| **GPU** | Mali-G2 Pro MC4 <br> Arm CSS for Mobile, Avalon (5th-gen GPU architecture) <br> Up to 1.1 GHz (expected) · 1.23 TFLOPS FP32 <br> Hardware virtualization, up to 16 VMs · L2 cache, shared 4 MB SLC |
| **NPU** | Rockchip NPU, 44 TOPS sparse INT8 (8.8 TOPS per core) <br> INT2/INT3/INT4/INT6/INT8/INT16 · FP4/FP6/FP8/FP16 <br> W1.58A8, W2A8, W2A16, W4A8, W4A16 <br> Caffe, TFLite, PyTorch, ONNX, Android NN <br> CNN and Transformer together · GRID-sample · MoE · speculative sampling |
| **VPU** | H.265/H.264/VP9/AV1/AVS2 decode up to 8K@120fps <br> H.264/H.265 encode up to 8K@60fps, 10-bit / YUV444 <br> VPSS · VDPP (picture quality) · AVSP (any-view stitching) · FEC (fisheye correction) · DFS (depth from stereo) |
| **Display** | Up to 2× 8K@60fps or 6× 4K@60fps <br> 2× HDMI 2.1 / eDP 1.4 / DP combo with DSC <br> 1× MIPI DSI, 4-lane, with DSC <br> USB Type-C with USB 3.2 Gen 2×1 and DisplayPort |
| **ISP** | 2× 24 MP + 1× 16 MP ISP <br> HDR and 3DNR, 140 dB HDR, LED flicker mitigation, 4-cell, FEC <br> 4× MIPI CSI-2 (1×4-lane/3-trio or 2×2-lane/2-trio, C-PHY/D-PHY) + DVP |
| **Connectivity** | USB 3.2 10 Gbit/s DRD (Type-C and DisplayPort) <br> USB 2.0 OTG + 2× USB 2.0 host <br> PCIe 5.0, 4 controllers (1×4-lane + 2×2-lane, 2×1-lane) <br> PCIe 3.0, 5 controllers (1×4-lane, 2×2-lane, 2×1-lane) <br> Three 10 Gbit/s PHYs shared by PCIe 3.0, SATA, USB 3.0, DP, and XGMII <br> Controllers: quad SATA 3.1, dual USB 3.0 DRD, dual XGMII · dual RGMII <br> I2C, I3C, SPI, UART, GPIO, 6× CAN, DSMC |
| **Audio** | SAI, 20 lanes · 20-channel ASRC · 2× 8-channel PDM |
| **Safety** | Dual Cortex-M52 with DCLS · error detection · BIST · secure boot and fast boot <br> ARM TrustZone (secure boot/JTAG, key ladder, cipher, HDCP) |
| **Package** | TBD, 0.65 mm ball pitch |
| **Availability** | Engineering samples in Q1 2027 |

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
