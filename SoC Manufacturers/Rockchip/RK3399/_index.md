---
weight: 10
title: Rockchip RK3399
soc:
- RK3399
tags:
- SOC-RK
summary: Rockchip RK3399 hexa-core (2× Cortex-A72 + 4× Cortex-A53), Mali-T860 MP4 GPU, 4K60 decode, PCIe 2.1 x4, dual USB-C with DisplayPort.
---
# Rockchip RK3399

The RK3399 was Rockchip's flagship before the RK3588. It has two Cortex-A72 and four Cortex-A53 cores, a Mali-T860 MP4, PCIe 2.1 x4 and two USB 3.0 Type-C ports with DisplayPort. Mainline support is mature: Panfrost handles the GPU and Hantro handles video decode. Libre Computer uses it on the Renegade Elite.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [x] Fully supported
- [ ] Works but not all features are implemented
- Libre Computer boards on this SoC boot upstream Linux and U-Boot
- The Mali-T860 GPU is supported by the Mesa Panfrost driver

---

## Documentation

- [Renegade Elite specifications (Libre Computer)](https://libre.computer/products/roc-rk3399-pc/)

---

## Boards with Rockchip RK3399

{{< taglist tag="RK3399" style="cards" >}}
