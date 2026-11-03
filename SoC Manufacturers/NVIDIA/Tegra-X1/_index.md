---
weight: 6
title: NVIDIA Tegra X1 (T210)
soc:
- T210
- Tegra-X1
tags:
- SOC-NVIDIA-Jetson
summary: "NVIDIA Tegra X1 (T210) - quad Cortex-A57 with a Maxwell GPU, used on the Jetson Nano and Jetson TX1 (and the Nintendo Switch)."
---
# NVIDIA Tegra X1 (T210)

The Tegra X1 (T210) is NVIDIA's 20 nm Maxwell-generation SoC, also known from the Nintendo Switch and the Shield TV. Jetson boards use only its four Cortex-A57 cores. The Jetson TX1 has the full 256-core GPU, while the low-cost Jetson Nano uses a 128-core version at a lower clock.

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

- [Jetson Nano Developer Kit (NVIDIA)](https://developer.nvidia.com/embedded/jetson-nano-developer-kit)

---

## Boards with NVIDIA Tegra X1 (T210)

{{< taglist tag="T210" style="cards" >}}
