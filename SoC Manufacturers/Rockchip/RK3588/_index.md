---
weight: 2
title: Rockchip RK3588
#bookCollapseSection: true
soc-series:
- RK35XX
soc:
- RK3588
tags: 
- SOC-RK
summary: Rockchip RK3588 flagship ARM processor - 8-core CPU (4x Cortex-A76 + 4x A55), Mali-G610 MP4 GPU, 6 TOPS NPU, 8K video decode, PCIe 3.0, USB 3.0.
---
# Rockchip RK3588

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}
<br>
{{% details title="Block Diagram" open=false %}}

![RK3588 Block Diagram](images/RK3588-Block-Diagram.jpg?f=webp)

{{% /details %}}

---

## Memory Speed

Board pages list the data rate of the RAM chips, e.g. LPDDR4X-4266. The speed the memory actually runs at is set by the DDR init blob from Rockchip's [rkbin](https://github.com/rockchip-linux/rkbin/tree/master/bin/rk35), which is built into U-Boot:

| rkbin DDR blob | LPDDR4/4X | LPDDR5 |
|---|---|---|
| `rk3588_ddr_lp4_2112MHz_lp5_2400MHz` (default) | 2112 MHz = 4224 MT/s | 2400 MHz = 4800 MT/s |
| `rk3588_ddr_lp4_1848MHz_lp5_2112MHz` | 1848 MHz = 3696 MT/s | 2112 MHz = 4224 MT/s |

So an LPDDR4X-4266 board on the default blob runs at 4224 MT/s. The frequency is in the blob's file name, so check which blob your board's U-Boot uses.

---

## Linux Support
{{% columns %}}
- ### Vendor BSP
  - Current Version (rkr5) based on: 6.1
  - Legacy: 5.10 <br>(versions do not compare to mainline)

- ### Mainline kernel
  - [ ] Fully supported
  - [x] Works but not all features are implemented.

  See [Mainline Status](https://gitlab.collabora.com/hardware-enablement/rockchip-3588/notes-for-rockchip-3588/-/blob/main/mainline-status.md?ref_type=heads)

{{% /columns %}}

---

## Variants

- [RK3588s](variants/rk3588s/)

## Documentation
- Technical Reference Manual

---

## Boards with RK3588

List of boards:

{{< taglist tag="RK3588" style="cards" >}}