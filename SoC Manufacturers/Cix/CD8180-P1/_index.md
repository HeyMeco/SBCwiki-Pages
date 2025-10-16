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
| **VPU** | - 8K@60fps decoder AV1, H.265, H.264, VP9, VP8, H.263, MPEG‑4, MPEG‑2<br>- 8K@30fps encoder H.265, H.264, VP9, VP8               |
| **NPU** | Neural Processing Unit (NPU)<br>- Computing Power: 30 TOPs<br>- Precision Support: INT4 / INT8 / INT16 / FP16 / TF32             |

{{% /details %}}
<br>
{{% details title="Block Diagram" open=false %}}

![P1 Block Diagram](images/P1-system-block-diagram.webp)

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented.

See [Mailing list](http://lore.kernel.org/lkml/?q=Cix+P1)
See [Community support status tracker](https://github.com/System64fumo/linux/blob/main/hardware/devices/arm/radxa/orion/orion.md)


---

## Boards with CD8180 / P1

List of boards:

{{< taglist CD8180 >}}

---

## CD8160

| **SoC** | **CD8160 (binned variant)**                                                                                                                  |
|---------|----------------------------------------------------------------------------------------------------------------------------------|
| **CPU** | 4x Cortex®-A720 (Big cores) up to **2.6GHz**<br>4x Cortex®‑A720 (Medium cores) up to 2.4GHz<br>4x Cortex®‑A520 (LITTLE cores) 1.8GHz |
| **Other differences** | Possibly less I/O like PCIe lanes (needs to be confirmed) |

## Boards with CD8160
- Radxa Orion O6N
- OrangePi 6 Plus