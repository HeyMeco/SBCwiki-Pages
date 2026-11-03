---
weight: 2
title: Amlogic S905D3
soc:
- S905D3
tags:
- SOC-Amlogic
summary: Amlogic S905D3 quad-core Cortex-A55, Mali-G31 GPU, 1.2 TOPS NPU, 4K60 decode and 1080p60 H.265 encode.
---
# Amlogic S905D3

The S905D3 is part of Amlogic's SM1 family, next to the S905X3. It has four Cortex-A55 cores, a Mali-G31 GPU and a 1.2 TOPS NPU. Libre Computer uses it on the Solitude board and the Solitude compute module.

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
- The Mali-G31 GPU is supported by the Mesa Panfrost driver

---

## Documentation

- [Solitude specifications (Libre Computer)](https://libre.computer/products/aml-s905d3-cc/)

---

## Boards with Amlogic S905D3

{{< taglist tag="S905D3" style="cards" >}}
