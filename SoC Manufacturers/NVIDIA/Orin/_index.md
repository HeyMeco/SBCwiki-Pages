---
weight: 3
title: NVIDIA Jetson Orin (T234)
soc:
- T234
- AGX-Orin
- Orin-NX
- Orin-Nano
tags:
- SOC-NVIDIA-Jetson
summary: "NVIDIA Jetson Orin (T234) - up to 12 Cortex-A78AE cores, Ampere GPU with up to 2,048 CUDA cores, up to 64 GB LPDDR5, up to 275 TOPS. AGX Orin, Orin NX and Orin Nano modules."
---
# NVIDIA Jetson Orin (T234)

Orin (T234) is NVIDIA's 8 nm Ampere-generation Jetson SoC, sold as three module families. **AGX Orin** uses a 699-pin connector. **Orin NX** and **Orin Nano** are small 260-pin SO-DIMM modules. Since JetPack 6.1 the "Super" power modes raise the CPU, GPU and memory clocks on Orin NX and Orin Nano. Those boosted figures are listed in the notes. Orin Nano has no hardware video encoder and no DLA.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Vendor BSP
- NVIDIA JetPack / Jetson Linux (Ubuntu-based) with CUDA, cuDNN and TensorRT

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented (Tegra platform support upstream; GPU acceleration needs NVIDIA's driver stack)

---

## Documentation

- [Jetson AGX Orin technical brief](https://www.nvidia.com/content/dam/en-zz/Solutions/gtcf21/jetson-orin/nvidia-jetson-agx-orin-technical-brief.pdf)
- [Jetson modules comparison](https://developer.nvidia.com/embedded/jetson-modules)

---

## Boards with NVIDIA Jetson Orin (T234)

{{< taglist tag="T234" style="cards" >}}
