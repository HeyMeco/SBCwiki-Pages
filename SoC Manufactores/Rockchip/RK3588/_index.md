---
weight: 1
title: Rockchip RK3588
#bookCollapseSection: true
soc-series:
- RK35XX
soc:
- RK3588
tags: 
- SOC-RK
---
# Rockchip RK3588

## General Specifications
{{< details title="Specs" open=true >}}

| **SoC** | **Rockchip RK3588**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Octa-core: <br> Quad-core ARM Cortex-A76(up to 2.4GHz) <br> Quad-core ARM Cortex-A55 (up to 1.8GHz)            |
| **RAM** | Dual Channel LPDDR4X/5                                                                                         |
| **GPU** | Mali-G610 MP4, compatible with OpenGLES 1.1, 2.0, and 3.2, OpenCL up to 2.2 and Vulkan1.2                      |
| **VPU** | 8K@60fps H.265 and VP9 decoder <br> 8K@30fps H.264 decoder <br> 4K@60fps AV1 decoder <br> 8K@30fps H.264 and H.265 encoder |
| **NPU** | 6TOPs, supports INT4/INT8/INT16/FP16                                                                           |

{{< /details >}}
<br>
{{< details title="Block Diagram" open=false >}}

![RK3588 Block Diagram](images/RK3588-Block-Diagram.jpg?f=webp)

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

See [Mainline Status](https://gitlab.collabora.com/hardware-enablement/rockchip-3588/notes-for-rockchip-3588/-/blob/main/mainline-status.md?ref_type=heads)

{{< /columns >}}

---

## Variants

- [RK3588s](variants/rk3588s/)

## Documentation
- Technical Reference Manual

---

## Boards with RK3588

List of boards:

{{< taglist RK3588 >}}