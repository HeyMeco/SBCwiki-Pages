---
weight: 2
title: NVIDIA Jetson Thor (T264)
soc:
- T264
- T5000
- T4000
- T3000
tags:
- SOC-NVIDIA-Jetson
summary: "NVIDIA Jetson Thor (T264) - up to 14 Arm Neoverse-V3AE cores, Blackwell GPU with up to 2,560 CUDA cores, up to 128 GB LPDDR5X at 273 GB/s, up to 2070 FP4 TFLOPS."
---
# NVIDIA Jetson Thor (T264)

Jetson Thor is NVIDIA's Blackwell-generation robotics platform, available since August 2025. The flagship **T5000** module pairs 14 Neoverse-V3AE cores with a 2,560-core Blackwell GPU and 128 GB of LPDDR5X. The **T4000** is a cut-down version with 64 GB. Both share the 699-pin connector, 256-bit memory bus and 273 GB/s bandwidth. In July 2026 NVIDIA announced the smaller **T3000** (and a reported T2000) for Q1 2027.

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

- [Introducing NVIDIA Jetson Thor (NVIDIA blog)](https://developer.nvidia.com/blog/introducing-nvidia-jetson-thor-the-ultimate-platform-for-physical-ai/)
- [Jetson Thor series modules datasheet](https://developer.nvidia.com/downloads/assets/embedded/secure/jetson/thor/docs/jetson-thor-series-modules-datasheet_ds-11945-001.pdf)

---

## Boards with NVIDIA Jetson Thor (T264)

{{< taglist tag="T264" style="cards" >}}
