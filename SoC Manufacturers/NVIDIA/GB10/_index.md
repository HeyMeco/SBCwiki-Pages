---
weight: 1
title: NVIDIA GB10 (DGX Spark)
soc:
- GB10
tags:
- SOC-NVIDIA-DGX
summary: NVIDIA GB10 Grace Blackwell superchip - 20-core Arm CPU (10× Cortex-X925 + 10× Cortex-A725), Blackwell GPU with 6,144 CUDA cores, 128 GB LPDDR5X at 273 GB/s.
---
# NVIDIA GB10 (DGX Spark)

The GB10 is the Grace Blackwell superchip in the DGX Spark and its OEM versions. It was co-developed with MediaTek. A 20-core Arm CPU and a Blackwell GPU share up to 128 GB of coherent LPDDR5X over a 256-bit bus. NVIDIA rates it at up to 1 PFLOP of sparse FP4 AI compute.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Vendor BSP
- DGX OS, NVIDIA's customized Ubuntu 24.04 with the NVIDIA kernel and driver stack

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented (GPU needs NVIDIA's driver)

---

## Documentation

- [DGX Spark product page](https://www.nvidia.com/en-us/products/workstations/dgx-spark/)

---

## Boards with NVIDIA GB10

{{< taglist tag="GB10" style="cards" >}}
