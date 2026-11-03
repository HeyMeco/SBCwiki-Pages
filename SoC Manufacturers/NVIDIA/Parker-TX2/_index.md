---
weight: 5
title: NVIDIA Jetson TX2 (T186 / Parker)
soc:
- T186
- Parker
- TX2
tags:
- SOC-NVIDIA-Jetson
summary: "NVIDIA Jetson TX2 (T186 Parker) - 2× NVIDIA Denver 2 + 4× Cortex-A57, 256-core Pascal GPU, 8 GB LPDDR4 at 59.7 GB/s."
---
# NVIDIA Jetson TX2 (T186 / Parker)

The T186, codenamed Parker, powers the Jetson TX2 module from 2017. It combines two of NVIDIA's own Denver 2 cores with four Cortex-A57 cores and a 256-core Pascal GPU. The TX2 module uses a 400-pin connector.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Vendor BSP
- NVIDIA JetPack / Jetson Linux (L4T); this generation no longer receives new JetPack major releases

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented (Tegra support upstream; Nouveau for the GPU)

---

## Documentation

- [Jetson TX2 announcement (NVIDIA blog)](https://developer.nvidia.com/blog/jetson-tx2-delivers-twice-intelligence-edge/)

---

## Boards with NVIDIA Jetson TX2 (T186 / Parker)

{{< taglist tag="T186" style="cards" >}}
