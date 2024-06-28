---
weight: 2
title: Rockchip RK3568
#bookCollapseSection: true
soc-series:
- RK35XX
soc:
- RK3568
tags: 
- SOC-RK
---
# Rockchip RK3568

## General Specifications
{{< details title="Specs" open=true >}}

| **SoC** | **Rockchip RK3568**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Quad-core ARM Cortex-A55 (up to 2GHz)            |
| **RAM** | 32bit LPDDR4/4X/3 | DDR4/3/3L with ECC support                                                                                     |
| **GPU** | Mali-G52EE, compatible with OpenGL® ES 1.1/2.0/3.2, OpenCL™ 2.0 and Vulkan® 1.1               |
| **VPU** | 4Kp60 H.264/H.265/VP9 decoder <br> 1080p60 H.264/H.265 encoder |
| **NPU** | 1TOPs, supports INT8/INT16/FP16/BFP16                                                                           |

{{< /details >}}
<br>
{{< details title="Block Diagram" open=false >}}

![RK3568 Block Diagram](images/RK3568-Block-Diagram.jpeg?f=webp)

{{< /details >}}

---

## Linux Support
{{< columns >}}
### Vendor BSP
- Current Version based on: 6.1
- Legacy: 5.10 <br>(versions do not compare to mainline)

<--->

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented.

{{< /columns >}}

---

## Variants

- RK3568J | Industrial Grade Version

## Documentation
- Technical Reference Manual

---

## Boards with RK3568

List of boards:

{{< taglist RK3568 >}}