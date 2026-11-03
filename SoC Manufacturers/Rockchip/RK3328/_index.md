---
weight: 11
title: Rockchip RK3328
soc:
- RK3328
tags:
- SOC-RK
summary: Rockchip RK3328 quad-core Cortex-A53, Mali-450 MP2 GPU, 4K60 H.265/H.264/VP9 decode, USB 3.0 and Gigabit Ethernet.
---
# Rockchip RK3328

The RK3328 is Rockchip's 64-bit TV box SoC with four Cortex-A53 cores, a Mali-450 MP2, 4K60 decode, USB 3.0 and Gigabit Ethernet. It is common on router and media boards, and Libre Computer uses it on the Renegade.

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
- The Mali-450 GPU is supported by the Mesa Lima driver

---

## Documentation

- [Renegade specifications (Libre Computer)](https://libre.computer/products/roc-rk3328-cc/)

---

## Boards with Rockchip RK3328

{{< taglist tag="RK3328" style="cards" >}}
