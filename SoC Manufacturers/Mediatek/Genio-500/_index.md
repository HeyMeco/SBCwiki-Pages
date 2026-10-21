---
weight: 4
title: Genio 500 / MT8385
soc-series:
- Genio
soc:
- Genio-500
- MT8385
tags:
- SOC-MTK
summary: MediaTek Genio 500 (MT8385) 12 nm IoT SoC — 4x Cortex-A73 + 4x A53, Mali-G72 MP3, dual VP6 VPU at 0.75 TOPS, FHD+ display and 32 MP camera.
---
# Genio 500 / MT8385

The MediaTek Genio 500 is a 12 nm octa-core IoT application processor for portable, home, and commercial devices that need stronger CPUs than Genio 350, with FHD+ displays and multi-camera vision. It pairs four Cortex-A73 cores with four Cortex-A53 cores and a dual VP6 vision DSP.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **MediaTek Genio 500 / MT8385** |
|---------|---------------------------------|
| **Process** | 12 nm |
| **CPU** | Octa-core:<br>4× Arm Cortex-A73 @ 2.0 GHz<br>4× Arm Cortex-A53 @ 2.0 GHz |
| **RAM** | LPDDR3 or LPDDR4/X up to 3733 Mbps<br>Up to 8 GB |
| **GPU** | Arm Mali-G72 MP3 @ up to 800 MHz<br>OpenGL ES 3.2, Vulkan 1.0, OpenCL 2.x |
| **NPU** | Dual-core Cadence Tensilica VP6 @ up to 525 MHz<br>About 0.75 TOPS |
| **VPU** | **Decode:** H.264/HEVC 1080p30<br>**Encode:** H.264 1080p30 |
| **Display** | Concurrent dual display<br>MIPI-DSI 4-lane, DPI/DBI<br>Up to FHD+ (2400×1080) |
| **ISP** | Up to 32 MP @ 30 fps<br>Multi-camera MIPI CSI-2 |
| **Storage** | eMMC 5.1, UFS 2.1 (1-lane), SD |
| **USB** | SuperSpeed USB device or USB 2.0 OTG |
| **Connectivity** | External Wi-Fi / Bluetooth / GNSS / FM via companion chips (e.g. MT7668 / MT6631) |
| **Temperature** | Typical modules: about −20°C to 85°C ambient |

{{% /details %}}

### Variant Differences

- **MT8385**: Primary Genio 500 application processor. Android, Yocto Linux, and Ubuntu are the usual OS options from MediaTek and module vendors.

---

## Linux Support

### Mainline kernel

- [ ] Fully supported
- [x] Vendor / BSP kernels are the common path (Yocto Kirkstone-era BSPs on modules)

---

## Resources

- [Genio 500 product page](https://www.mediatek.com/products/iot/genio-iot/genio-500)
- [MT8385 datasheet (MediaTek)](https://www.mediatek.com/hubfs/MediaTek%20Assets/Pdfs/Genio%20Documents/MTK_MT8385_IoT_Application_Processor_Datasheet_v1.4.pdf)

---

## Boards with Genio 500

List of boards:

{{< taglist tag="Genio-500" style="cards" >}}

{{< taglist tag="MT8385" style="cards" >}}
