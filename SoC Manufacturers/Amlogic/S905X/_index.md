---
weight: 4
title: Amlogic S905X
soc:
- S905X
tags:
- SOC-Amlogic
summary: Amlogic S905X quad-core Cortex-A53, Mali-450 MP3 GPU, 4K60 H.265/VP9 decode, HDMI 2.0 with HDR.
---
# Amlogic S905X

The S905X is Amlogic's GXL-family 4K TV box SoC. It has four Cortex-A53 cores, a Mali-450 MP3 and 4K60 H.265 and VP9 decode. It has had mainline Linux support for years, and Libre Computer uses it on the Le Potato and Sweet Potato.

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

- [Le Potato specifications (Libre Computer)](https://libre.computer/products/aml-s905x-cc/)

---

## Boards with Amlogic S905X

{{< taglist tag="S905X" style="cards" >}}
