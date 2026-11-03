---
weight: 1
title: Sophgo BM1688
soc:
- BM1688
tags:
- SOC-Sophgo
summary: Sophgo BM1688 - octa-core Cortex-A53 at up to 1.65 GHz, 16 TOPS INT8 TPU, 16-channel 1080p30 decode, up to six camera inputs.
---
# Sophgo BM1688

The BM1688 is Sophgo's edge vision AI SoC. Eight Cortex-A53 cores and a RISC-V C906 coprocessor sit next to Sophgo's own TPU, rated at 16 TOPS INT8 or 32 TOPS INT4. Its video engine decodes up to 16 1080p30 streams at once, which makes it suited to multi-camera video analytics.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Vendor BSP
- Sophgo SDK with Linux BSP and the TPU-MLIR toolchain
- Orange Pi images for the Orange Pi O1

### Mainline kernel
- [ ] Fully supported
- [ ] Works but not all features are implemented
- No mainline support documented

---

## Documentation

- [Sophgo website](https://www.sophgo.com/)
- [LinuxGizmos: Orange Pi O1 with BM1688](https://linuxgizmos.com/16-tops-ai-sbc-with-sata-3-0-runs-on-octa-core-sophgo-bm1688/)

---

## Boards with Sophgo BM1688

{{< taglist tag="BM1688" style="cards" >}}
