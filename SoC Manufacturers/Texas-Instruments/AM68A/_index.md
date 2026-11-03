---
weight: 2
title: TI AM68 / AM68A
soc:
- AM68
- AM68A
tags:
- SOC-TI
summary: TI AM68A vision processor - dual Cortex-A72 at 2 GHz, 8 TOPS C7x/MMA deep-learning accelerator, BXS-4-64 GPU, 480 MP/s ISP. AM68 is the variant without AI.
---
# TI AM68 / AM68A

The AM68A (J721S2 family) is TI's mid-range vision AI processor. It has two Cortex-A72 cores, Cortex-R5F real-time cores, an 8 TOPS C7x/MMA accelerator that can only run deep-learning workloads, and a VPAC ISP. The AM68 is the general-purpose version without AI acceleration. Both run on the [SK-AM68](boards/ti-sk-am68/) starter kit.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Vendor BSP
- TI Processor SDK Linux (11.00, May 2025) and Edge AI SDK
- Armbian community images for the SK boards

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented (K3 J721S2 / J784S4 platforms)
- The BXS-4-64 GPU is supported by the open-source PowerVR (`imagination`) Mesa and kernel drivers, which are under active development

---

## Documentation

- [AM68A product page](https://www.ti.com/product/AM68A)
- [AM68x datasheet](https://www.ti.com/lit/ds/symlink/am68.pdf)

---

## Boards with TI AM68 / AM68A

{{< taglist tag="AM68A" style="cards" >}}
