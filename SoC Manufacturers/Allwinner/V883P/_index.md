---
weight: 4
title: Allwinner V883P
#bookCollapseSection: true
aliases:
- /docs/soc-manufacturers/allwinner/v883/
soc-series:
- V
soc:
- V883
- V883P
tags:
- SOC-Allwinner
- V883
- V883P
summary: Allwinner V883P RISC-V vision SoC - Quad-core XuanTie C907 up to 1.8GHz, E907 MCU, 4 TOPS NPU, 4K@75fps H.265 encoding, AI-ISP, up to 16 cameras.
---
# Allwinner V883P

The V883P is the full part of Allwinner's V883 RISC-V vision and imaging SoC series, announced on 6 November 2026 together with a V883 vision development PDK. It has four XuanTie C907 RISC-V cores, a XuanTie E907 RISC-V MCU, a 4 TOPS NPU and video up to 4K@75fps. Allwinner targets action and handheld cameras, dashcams, AI streaming cameras, multi-channel edge vision and industrial machine vision. The cut-down [V883M](/docs/soc-manufacturers/allwinner/v883m/) is pin-to-pin compatible, so one board design can carry either part.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

> Source notes: Allwinner publishes its product-page spec table for "V883", and its headline figures (4 TOPS, 4K@75fps) are the V883P's. Allwinner's launch post names USB 3.0, while the product page lists USB 3.1. CAN-FD appears in the launch post but not in the product page's interface list. The launch post describes the display output as 2× 2-lane MIPI-DSI; the product page lists 1× 4-lane or 2× 2-lane. Allwinner has not published the process node, package or maximum memory size.

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [ ] Works but not all features are implemented.

Allwinner supplies the V883 series with Tina Linux, its own Linux BSP, and a V-series SDK. No mainline support has been announced.

---

## Documentation
- Technical Reference Manual

---

## Resources

- [Allwinner V883 product page](https://www.allwinnertech.com/index.php?c=product&a=index&id=151)
- [Allwinner launch post: V883 series and V883 vision PDK (2026-11-06, Chinese)](https://mp.weixin.qq.com/s/_6GTz22fvzGd1CGJVk6TRw)
- [Allwinner preview post: V883 (2026-10-15, Chinese)](https://mp.weixin.qq.com/s/RVEFmZTHxqSQOhNNYfNOnA)
- [IoT World: V883 launch coverage (Chinese)](https://www.iotworld.com.cn/html/News/202611/2f3ce348e427e4de.shtml)
- [Top1Chip: V883 series announcement](https://www.top1chip.com/blog/51467)
- [Allwinner newsroom](https://www.allwinnertech.com/index.php?c=news)

---

## Boards with V883P

List of boards:

{{< taglist tag="V883P" style="cards" >}}
