---
weight: 5
title: Genio 350 / MT8365
soc-series:
- Genio
soc:
- Genio-350
- MT8365
tags:
- SOC-MTK
summary: MediaTek Genio 350 (MT8365) entry 14 nm IoT SoC — quad Cortex-A53, Mali-G52, 0.35 TOPS VP6, HiFi 4 DSP, dual FHD display.
---
# Genio 350 / MT8365

The MediaTek Genio 350 is the entry multimedia IoT platform in the Genio line. It uses four Cortex-A53 cores on 14 nm, with a Mali-G52 GPU, a VP6 vision DSP, and a HiFi 4 audio DSP. MediaTek positions it for cost-sensitive smart home, retail, and industrial devices that still need dual display and camera support.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **MediaTek Genio 350 / MT8365** |
|---------|---------------------------------|
| **Process** | 14 nm |
| **CPU** | 4× Arm Cortex-A53 @ 2.0 GHz |
| **RAM** | x32 LPDDR3-1600 up to 4 GB<br>x32 LPDDR4X-3200 up to 4 GB |
| **GPU** | Arm Mali-G52 @ 800 MHz<br>OpenGL ES 3.2, Vulkan 1.1, OpenCL 2.0 |
| **NPU** | 0.35 TOPS (1× Tensilica VP6) |
| **Audio DSP** | Tensilica HiFi 4 |
| **VPU** | **Decode:** H.264/H.265/MPEG4 FHD60<br>**Encode:** H.264/H.265 FHD60 |
| **Display** | Dual: max FHD+HD<br>Single: max FHD<br>1× MIPI-DSI (4L), 1× DPI / LVDS |
| **ISP** | 1× ISP, 13 MP @ 30 fps<br>2× MIPI CSI-2 (4L) |
| **Storage** | eMMC 5.1, SD 3.0, SPI-NAND |
| **USB** | 1× USB 2.0 Host, 1× USB 2.0 Host/Device |
| **Ethernet** | 10/100 MAC (RMII) |
| **Connectivity** | Integrated Wi-Fi 5 1x1 / Bluetooth 5.0 baseband (MT6631)<br>External 2x2 Wi-Fi options |
| **Package** | VFBGA 12.2 × 11.8 × 0.9 mm |
| **Temperature** | −20°C to 105°C (Tj) |
| **Longevity** | Available until 2030 |

{{% /details %}}

---

## Linux Support

### Mainline kernel

- [ ] Fully supported
- [x] Android, IoT Yocto, and Ubuntu are supported through MediaTek and partners

---

## Resources

- [Genio 350](https://genio.mediatek.com/genio-350)
- [MT8365 datasheet (MediaTek)](https://www.mediatek.com/hubfs/MediaTek%20Assets/Pdfs/Genio%20Documents/MTK_MT8365_IoT_Application-Processor_Datasheet_v1.5.pdf)

---

## Boards with Genio 350

List of boards:

{{< taglist tag="Genio-350" style="cards" >}}

{{< taglist tag="MT8365" style="cards" >}}
