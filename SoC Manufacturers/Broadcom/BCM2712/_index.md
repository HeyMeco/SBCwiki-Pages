---
title: Broadcom BCM2712
weight: 1
soc:
- BCM2712
tags:
- SOC-Broadcom
summary: Broadcom BCM2712 - The SoC powering the Raspberry Pi 5, Pi 500, Pi 500+ and Compute Module 5 with quad-core Cortex-A76
---
# Broadcom BCM2712

The BCM2712 is the quad-core Cortex-A76 SoC that Broadcom makes for Raspberry Pi. It powers the Raspberry Pi 5, the Pi 500 and 500+ keyboard computers, and the Compute Module 5. PCIe, USB 3, Ethernet and most low-speed I/O sit on the separate RP1 southbridge.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented
- Raspberry Pi OS uses the Raspberry Pi downstream kernel

---

## Boards with BCM2712

{{< taglist tag="BCM2712" style="cards" >}}
