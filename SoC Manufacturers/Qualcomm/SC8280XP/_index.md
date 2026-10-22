---
weight: 20
title: Snapdragon 8cx Gen 3
soc-series:
- Snapdragon
soc:
- SC8280XP
tags: 
- SOC-Qualcomm
- Snapdragon
summary: Qualcomm Snapdragon 8cx Gen 3 (SC8280XP) compute platform - 4x Cortex-X1 and 4x Cortex-A78 up to 3.0GHz, Adreno 690 GPU, Qualcomm AI Engine up to 29+ TOPS, 4K120 video.
---
# Snapdragon 8cx Gen 3

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

### Also known as:

- SC8280XP
- SA8540P
- SA8295P

---

## Resources:

- [SC8280XP mainline status](https://linux-msm.github.io/mainline-status/soc/sc8280xp)

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [x] Works, but not every feature is implemented. Driver support matrix is [here](https://linux-msm.github.io/mainline-status/soc/sc8280xp)

### Mesa GPU support
- [x] Available with [Freedreno](https://docs.mesa3d.org/drivers/freedreno.html) (Adreno 690)

## Windows on Arm Support
- [Available](https://learn.microsoft.com/en-us/windows-hardware/design/minimum/supported/windows-11-24h2-supported-qualcomm-processors) but depends on the board vendor to provide a compatible bootloader

---

## Boards with Snapdragon 8cx Gen 3

List of boards:

{{< taglist tag="SC8280XP" style="cards" >}}
