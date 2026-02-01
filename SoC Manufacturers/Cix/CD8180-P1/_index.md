---
weight: 1
title: CD8180 / CD8160 / P1
#bookCollapseSection: true
soc-series:
- Filogic
soc:
- CD8180
- CD8160
tags: 
- SOC-Cix
summary: Cix CD8180/P1 - High-performance 12-core SoC with Immortalis G720 GPU and 30 TOPS NPU
---
# CD8180 / CD8160 / P1

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **CD8180 / P1**                                                                                                                  |
|---------|----------------------------------------------------------------------------------------------------------------------------------|
| **CPU** | 4x Cortex®-A720 (Big cores) up to 2.8GHz<br>4x Cortex®‑A720 (Medium cores) up to 2.4GHz<br>4x Cortex®‑A520 (LITTLE cores) 1.8GHz |
| **RAM** | LPDDR5 RAM<br>- 128bit memory bus<br>- 5500MT/s transfer speed<br>- Configurations: 4GB / 8GB / 16GB / 32GB / 64GB               |
| **GPU** | Arm® Immortalis™ G720 MC10<br>- Hardware Ray‑Tracing enabled<br>- Vulkan® 1.3<br>- OpenGL® ES 3.2<br>- OpenCL® 3.0               |
| **VPU** | Arm-China Linlon V8<br>- 8K@60fps decoder AV1, H.265, H.264, VP9, VP8, H.263, MPEG‑4, MPEG‑2<br>- 8K@30fps encoder H.265, H.264, VP9, VP8               |
| **NPU** | Arm-China Zhouyi<br>- Computing Power: 30 TOPs<br>- Precision Support: INT4 / INT8 / INT16 / FP16 / TF32             |

>[!NOTE]
>Every Cix P1 has been limited up to 2.6GHz afterwards while the original target was 2.8GHz

{{% /details %}}
<br>
{{% details title="Block Diagram" open=false %}}

![P1 Block Diagram](images/Cix-P1-Blockdiagram.webp)

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [ ] Fully supported.
- [x] Works but not all features are implemented.
- Driver support status available [here](https://github.com/cixtech/linux-mainline/wiki)

---

## Boards with Cix P1

List of boards:

{{< taglist tag="CD8180" style="cards" >}} 

- Minisforum MS-R1
- Radxa Orion O6N
- OrangePi 6 Plus
- MetaComputing ARM AI PC

---

## What variant is CD8160?

> “CD8160 was the silkscreen used in early mass production. As PC/server models entered production, all silkscreen numbers were standardized to C*8180. CD8160 is no longer supplied.”

Cix P1 variants like CD8160 are all the same SoC from different batches in production. There are **no differences**.
