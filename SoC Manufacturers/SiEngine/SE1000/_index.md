---
weight: 1
title: SiEngine SE1000
soc:
- SE1000
- SE1000-I
tags:
- SOC-SiEngine
summary: SiEngine SE1000 / SE1000-I - 7 nm octa-core (4× Cortex-A76 + 4× Cortex-A55), dual Mali-G76 GPUs, 6.8 TOPS Zhouyi NPU, 4K@120 decode.
---
# SiEngine SE1000

The SE1000 (Longying No. 1) is SiEngine's 7 nm automotive cockpit SoC. The SE1000-I is its industrial AIoT version, built with Arm China. It has two Mali-G76 GPUs, a dual-core Arm China [Zhouyi](/docs/soc-manufacturers/arm/zhouyi-npu/) NPU, two HiFi 5 DSPs and two ISPs. Functional-safety islands are rated up to ASIL-D.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Vendor BSP
- Ubuntu images from Radxa for the SiRider S1

### Mainline kernel
- [ ] Fully supported
- [ ] Works but not all features are implemented
- No mainline support documented

---

## Documentation

- [Radxa SiRider S1 product brief](https://dl.radxa.com/sirider/s1/radxa_sirider_s1_product_brief.pdf)

---

## Boards with SiEngine SE1000

{{< taglist tag="SE1000" style="cards" >}}
