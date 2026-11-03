---
weight: 2
title: Broadcom RP3A0
soc:
- RP3A0
- BCM2710A1
tags:
- SOC-Broadcom
summary: Broadcom RP3A0 - system-in-package with a quad-core Cortex-A53 BCM2710A1 at 1 GHz and 512 MB LPDDR2, used on the Raspberry Pi Zero 2 W.
---
# Broadcom RP3A0

The RP3A0 is a system-in-package that Raspberry Pi built for the Zero 2 W. It stacks 512 MB of LPDDR2 on a BCM2710A1, the same die as the Raspberry Pi 3's BCM2837, clocked at 1 GHz.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [x] Fully supported (BCM2837 / `bcm2710` family, `vc4` display and GPU driver)
- Raspberry Pi OS uses the Raspberry Pi downstream kernel

---

## Documentation

- [Raspberry Pi Zero 2 W product brief](https://datasheets.raspberrypi.com/rpizero2/raspberry-pi-zero-2-w-product-brief.pdf)

---

## Boards with Broadcom RP3A0

{{< taglist tag="RP3A0" style="cards" >}}
