---
weight: 1
title: Synaptics Astra SL1680
soc:
- SL1680
tags:
- SOC-Synaptics
summary: Synaptics Astra SL1680 - quad Cortex-A73 at 2.1 GHz, PowerVR GE9920 GPU, 7.9 TOPS NPU, 4K60 AV1 decode, HDMI 2.1 Tx and Rx.
---
# Synaptics Astra SL1680

The SL1680 is the top Astra SL-series processor. Its four Cortex-A73 cores deliver up to 40,000 DMIPS, next to a 7.9+ TOPS NPU and a PowerVR Series9XE GPU. It decodes 4K60 AV1 and has both HDMI 2.1 output and input. It targets smart home and industrial displays, signage, point-of-sale terminals and security gateways.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Vendor BSP
- Synaptics Astra Yocto SDK
- [Torizon](https://www.torizon.io/supported-hardware/synaptics) by Toradex, with quarterly releases

### Mainline kernel
- [ ] Fully supported
- [ ] Works but not all features are implemented
- No mainline support documented

---

## Documentation

- [SL1680 product brief](https://developer.senarytech.com/download/doc/AstraBrief/sl1680-product-brief.pdf)
- [SL1680 datasheet](https://www.mouser.com/datasheet/2/1622/Synaptics-3518973.pdf)

---

## Boards with Synaptics Astra SL1680

{{< taglist tag="SL1680" style="cards" >}}
