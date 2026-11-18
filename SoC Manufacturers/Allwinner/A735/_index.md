---
weight: 1
title: Allwinner A735
#bookCollapseSection: true
soc:
- A735
tags:
- SOC-Allwinner
- A735
summary: Allwinner A735 ARM processor - Octa-core hybrid (2x Cortex-A76 + 6x Cortex-A55) up to 2.2GHz, G310V5 GPU, 5 TOPS NPU, pin-compatible with A733.
---
# Allwinner A735

The A735 is an octa-core Allwinner tablet SoC, pin-to-pin compatible with the [A733](/docs/soc-manufacturers/allwinner/a733/), so A733 board designs can take it without a respin. Allwinner introduced it on 13 November 2026 together with an Android 17 product package; the A735 has passed Android 17 GMS certification. Allwinner targets tablets first, then tablet-like devices such as learning tablets, POS terminals and portable smart displays.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

> Source note: all figures come from Allwinner's A735 announcement. Allwinner has not published a datasheet, the process node, per-cluster clocks, video encode capability, the GPU's API versions or the NPU's datatypes. These are left out rather than copied from the A733.

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [ ] Works but not all features are implemented.

Allwinner lists Linux among the supported operating systems. No mainline support has been announced.

---

## Documentation
- Technical Reference Manual

---

## Resources

- [Allwinner announcement: A735 Android 17 product package (2026-11-13, Chinese)](https://mp.weixin.qq.com/s/KuMFdHYmSAiRP0EJjCTRiQ)
- [Allwinner newsroom](https://www.allwinnertech.com/index.php?c=news)

---

## Boards with A735

List of boards:

{{< taglist tag="A735" style="cards" >}}
