---
weight: 1
title: Arduino Ventuno Q
categories:
- board
tags: 
- QCS8275
boards:
- Arduino-Ventuno-Q
board-vendor:
- Arduino
summary: "Arduino Ventuno Q high-performance industrial SBC - Qualcomm Dragonwing IQ8 (QCS8275), STM32H5 MCU, 16GB LPDDR5, 64GB eMMC, M.2 NVMe, WiFi 6, 2.5GbE, and CAN-FD."
images:
- images/1-Arduino_VENTUNO_Q_Front_Render.webp
---

# Arduino Ventuno Q

## Board Pictures
{{< gallery match="images/*" sortOrder="asc" rowHeight="150" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=true previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware
{{% details title="Specs" open=true %}}

| **SoC** | **Qualcomm Dragonwing™ IQ8 (IQ-8275)** |
|:--- |:--- |
| **CPU** | Octa-Core:<br>2x Gold Prime @ 2.35 GHz <br>2x Gold @ 2.1 GHz <br>4x Silver @ 1.95 GHz) |
| **GPU/VPU** | Adreno 623 @ 877 MHz |
| **NPU** | Hexagon Tensor AI Processor: up to 40 dense TOPS |
| **ISP** | Qualcomm Spectra 692 ISP |
| **RAM** | 16GB LPDDR5 |
| **Storage** | 64GB eMMC<br>M.2 connector for NVMe Gen 4 external storage |

<br>

| **Microcontroller (MCU)** | **STM32H5F5** |
|:--- |:--- |
| **CPU** | Arm® Cortex® M33 @ 250MHz |
| **Flash** | 4MB |
| **RAM** | 1.5MB |
| **OS** | Arduino core on Zephyr |

---

### Interfaces

| **I/O** | Description |
|:--- |:--- |
| **Connectivity** | Wi-Fi® 6 2.4/5/6 GHz with onboard antenna<br>Bluetooth® 5.3 with onboard antenna<br>1x 2.5Gbit RJ45 Ethernet |
| **USB** | 1x USB-C port (host/device role switching, power role switch, video output)<br>2x USB 3.0 Type A<br>2x USB 3.0 on JOMEGA header |
| **Video** | 1x HDMI muxed with MIPI DSI on JMEDIA header<br>Video output (DP Alt mode) support via USB-C<br>MIPI DSI pins on JMEDIA header |
| **Camera** | USB camera support<br>3x MIPI CSI connectors muxed with 2x MIPI CSI on JMEDIA header |
| **Audio** | 2x Microphone IN / Headphone OUT / Ear OUT / Line OUT on JMISC header |
| **CAN** | 1x CAN-FD PHY on screw terminal<br>3x CAN-FD (no PHY) on JOMEGA header<br>1x CAN-FD (no PHY) on UNO Shield headers |
| **Power Supply** | USB-C connector (5 VDC max @ 3 A)<br>5.5x2.1 mm Power Jack (12-24 VDC)<br>Screw Terminal (7-24 VDC)<br>7-24 V on JOMEGA |
| **Dimensions** | 160 x 100 x 25.8 mm |

{{% /details %}}

## Available OS images
- Ubuntu
- Debian (Upstream)
- Arduino core on Zephyr (for MCU)

## Documentation / Links
- [Arduino Ventuno Q Product Page](https://www.arduino.cc/product-ventuno-q)

## Benchmarks
*No benchmarks available yet.*

## Guides
*No guides available yet.*

## Articles
*No articles available yet.*
