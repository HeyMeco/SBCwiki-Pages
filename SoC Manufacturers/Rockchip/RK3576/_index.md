---
weight: 2
title: Rockchip RK3576
#bookCollapseSection: true
soc-series:
- RK35XX
soc:
- RK3576
tags: 
- SOC-RK
summary: Rockchip RK3576 AIoT ARM processor - Octa-core hybrid (4x Cortex-A72 + 4x A53), Mali-G52 GPU, 6 TOPS NPU, 4K video decode.
---
# Rockchip RK3576

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **Rockchip RK3576**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Octa-core hybrid: <br> 4× ARM Cortex-A72 (up to 2.2GHz) <br> 4× ARM Cortex-A53 (up to 1.8GHz)            |
| **RAM** | 32-bit LPDDR4/LPDDR4X/LPDDR5                                                                                     |
| **GPU** | Mali-G52 MC3, compatible with OpenGL® ES 1.1/2.0/3.2, OpenCL™ 2.1 and Vulkan® 1.2               |
| **VPU** | 4K@120fps H.265/VP9/AV1/AVS2 decoder <br> 4K@60fps H.264 decoder <br> 4K@60fps H.264/H.265 encoder |
| **NPU** | 6TOPs, supports INT4/INT8/INT16/FP16/BF16/TF32                                                                           |

{{% /details %}}

---

## Linux Support
{{% columns %}}
- ### Vendor BSP
  - Current Version (rkr5) based on: 6.1
  - Legacy: 5.10 <br>(versions do not compare to mainline)

- ### Mainline kernel
  - [ ] Fully supported
  - [x] Works but not all features are implemented.

{{% /columns %}}

---

## Documentation
- Technical Reference Manual

---

## Boards with RK3576

List of boards:

{{< taglist tag="RK3576" style="cards" >}}
