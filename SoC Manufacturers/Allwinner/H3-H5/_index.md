---
weight: 5
title: Allwinner H2+ / H3 / H5
soc:
- H2-Plus
- H3
- H5
tags:
- SOC-Allwinner
summary: "Allwinner H2+, H3 and H5 - pin-compatible quad-core TV box SoCs: Cortex-A7 with Mali-400 MP2 (H2+/H3) or 64-bit Cortex-A53 with Mali-450 MP4 (H5)."
---
# Allwinner H2+ / H3 / H5

The H2+, H3 and H5 are pin-compatible Allwinner TV box SoCs, so one board design can carry any of them. The H2+ and H3 have four 32-bit Cortex-A7 cores and a Mali-400 MP2. The H2+ is limited to 1080p HDMI output. The H5 has four 64-bit Cortex-A53 cores and a Mali-450 MP4. All three have long-standing mainline Linux and U-Boot support from the linux-sunxi community.

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
- The Mali-400/450 GPUs are supported by the Mesa Lima driver

---

## Documentation

- [linux-sunxi: H3](https://linux-sunxi.org/H3)
- [linux-sunxi: H5](https://linux-sunxi.org/H5)

---

## Boards with Allwinner H2+ / H3 / H5

{{< taglist tag="H3" style="cards" >}}
