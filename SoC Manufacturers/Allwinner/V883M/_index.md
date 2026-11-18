---
weight: 5
title: Allwinner V883M
#bookCollapseSection: true
soc-series:
- V
soc:
- V883
- V883M
tags:
- SOC-Allwinner
- V883
- V883M
summary: Allwinner V883M RISC-V vision SoC - Quad-core XuanTie C907, E907 MCU, 3 TOPS NPU, 4K@55fps video, pin-to-pin compatible with V883P.
---
# Allwinner V883M

The V883M is the cut-down part of Allwinner's V883 RISC-V vision and imaging SoC series, announced on 6 November 2026 together with a V883 vision development PDK. Like the [V883P](/docs/soc-manufacturers/allwinner/v883p/), it has four XuanTie C907 RISC-V cores and a XuanTie E907 RISC-V MCU. It has a smaller NPU (3 TOPS instead of 4) and video up to 4K@55fps instead of 4K@75fps. It is pin-to-pin compatible with the V883P, so one board design can carry either part.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

> Source notes: Allwinner has not published a separate spec table for the V883M. This table only lists what Allwinner states for it; see the [V883P](/docs/soc-manufacturers/allwinner/v883p/) for the full V883 spec table.

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
- [Top1Chip: V883 series announcement](https://www.top1chip.com/blog/51467)
- [Allwinner newsroom](https://www.allwinnertech.com/index.php?c=news)

---

## Boards with V883M

List of boards:

{{< taglist tag="V883M" style="cards" >}}
