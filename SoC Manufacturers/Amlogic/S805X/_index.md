---
weight: 5
title: Amlogic S805X
soc:
- S805X
tags:
- SOC-Amlogic
summary: Amlogic S805X quad-core Cortex-A53, Mali-450 MP3 GPU, 1080p H.265/VP9 decode, 16-bit DDR3/DDR4.
---
# Amlogic S805X

The S805X is the 1080p member of Amlogic's GXL family (with the S905X and S905D). It has four Cortex-A53 cores, a Mali-450 MP3 and a 16-bit memory bus, and is limited to 1080p video. Libre Computer uses it on the La Frite and Das Frite.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [x] Fully supported
- [ ] Works but not all features are implemented
- Libre Computer boards on this SoC boot upstream Linux and U-Boot
- The Mali-450 GPU is supported by the Mesa Lima driver

---

## Documentation

- [La Frite specifications (Libre Computer)](https://libre.computer/products/aml-s805x-ac/)

---

## Boards with Amlogic S805X

{{< taglist tag="S805X" style="cards" >}}
