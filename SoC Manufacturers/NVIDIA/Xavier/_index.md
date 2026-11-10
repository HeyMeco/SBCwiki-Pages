---
weight: 4
title: NVIDIA Jetson Xavier (T194)
soc:
- T194
- AGX-Xavier
- Xavier-NX
tags:
- SOC-NVIDIA-Jetson
summary: "NVIDIA Jetson Xavier (T194) - up to 8 NVIDIA Carmel Armv8.2-A cores, Volta GPU with up to 512 CUDA cores, up to 32 TOPS. AGX Xavier and Xavier NX modules."
---
# NVIDIA Jetson Xavier (T194)

Xavier (T194) was NVIDIA's first Jetson SoC with Tensor Cores and DLA accelerators. Its CPU cores are NVIDIA's own Carmel cores (Armv8.2-A). It was sold as the **AGX Xavier** module (699-pin, 2018) and the SO-DIMM **Xavier NX** module (2020), and has been replaced by Orin.

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

- [Jetson AGX Xavier announcement (NVIDIA blog)](https://developer.nvidia.com/blog/nvidia-jetson-agx-xavier-32-teraops-ai-robotics/)

---

## Boards with NVIDIA Jetson Xavier (T194)

{{< taglist tag="T194" style="cards" >}}
