---
weight: 0
title: Genio 1200 / MT8395
#bookCollapseSection: true
soc-series:
- Genio
soc:
- Genio-1200
tags: 
- SOC-MTK
summary: MediaTek Genio 1200 (MT8395) high-performance edge AI platform - Octa-core (4x Cortex-A78 + 4x A55), Mali-G57 MC5, 4.8 TOPS NPU, triple 4K display, 6nm.
---
# Genio 1200 / MT8395

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **MediaTek Genio 1200 / MT8395**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **Process** | 6nm                                                                                     |
| **CPU** | Octa-core: <br> 4× Arm Cortex-A78 @ 2.2 GHz <br> 4× Arm Cortex-A55 @ 2.0 GHz            |
| **RAM** | x64 LPDDR4X-4266 (up to 16GB)                                                                                     |
| **GPU** | Arm Mali-G57 MC5 @ 880 MHz<br>OpenGL® ES 3.2, Vulkan® 1.1, OpenCL™ 2.0               |
| **NPU** | MediaTek 3rd Gen NPU: **4.8 TOPS**<br>(2× MDLA2.0 + 2× Tensilica VP6)                                                                           |
| **Audio DSP** | Cadence Tensilica HiFi 4 DSP                                                                           |
| **VPU** | **Decode:** H.264/H.265/AV1/VP9 (4K@90fps), MPEG4/VP8 (FHD@60fps)<br>**Encode:** H.264/H.265 (4K@60fps) |
| **Display** | Triple display: max 4K60+4K30+4K30<br>Dual display: max 4K60+4K60<br>Single: max 4K60<br>2× MIPI-DSI (4L), 1× eDP 1.4, 1× DP 1.4, 1× HDMI 2.0 |
| **ISP** | 2× ISP: 48MP @ 30fps or 16MP+16MP @ 30fps<br>3× MIPI CSI-2 4-lane (virtual: 6× FHD30), HDMI-RX |
| **Storage** | eMMC 5.1, UFS 2.1, SD 3.0, SPI-NOR                                                                           |
| **USB** | 2× USB 2.0 (Host/Device), 1× USB 3.2 Gen1 (Host/Device), 1× USB 3.2 Gen1 (Host, shared with PCIe 2.0)                                                                           |
| **Ethernet** | 1× GbE MAC (TSN)                                                                           |
| **PCIe** | 1× PCIe 2.0 (1L RC), 1× PCIe 3.0 (2L RC/EP)                                                                           |
| **Security** | ARM TrustZone, Secure Boot (RSA3072), Crypto Engine, RNG                                                                           |
| **Package** | VFBGA 15×15×0.9 mm, 0.4 mm ball pitch                                                                           |
| **Temperature** | Consumer: -20°C to 95°C (Tj)<br>Industrial: -40°C to 105°C (Tj)                                                                           |

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented.

---

## Documentation
- [MediaTek Genio 1200 – Product page](https://www.mediatek.com/products/iot/genio-iot/genio-1200)
- Technical Reference Manual (Genio Developer Center)

---

## Boards with Genio-1200

List of boards:

{{< taglist tag="Genio-1200" style="cards" >}}
