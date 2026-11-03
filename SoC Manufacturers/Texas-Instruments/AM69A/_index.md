---
weight: 1
title: TI AM69 / AM69A
soc:
- AM69
- AM69A
tags:
- SOC-TI
summary: TI AM69A vision processor - 8× Cortex-A72 at 2 GHz, 32 TOPS from four C7x/MMA accelerators, BXS-4-64 GPU, 1440 MP/s ISP, multi-port Ethernet switch.
---
# TI AM69 / AM69A

The AM69A (J784S4 family) is TI's top vision AI processor. It has eight Cortex-A72 cores and four C7x/MMAv2 deep-learning accelerators for up to 32 TOPS, and an ISP for up to 12 cameras. Its integrated Ethernet switch supports up to eight external ports, two of them at up to 10 Gbit/s. The AM69 is the general-purpose version. Both run on the [SK-AM69](boards/ti-sk-am69/) starter kit.

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

- [AM69A product page](https://www.ti.com/product/AM69A)
- [AM69A datasheet](https://www.ti.com/lit/ds/symlink/am69a.pdf)

---

## Boards with TI AM69 / AM69A

{{< taglist tag="AM69A" style="cards" >}}
