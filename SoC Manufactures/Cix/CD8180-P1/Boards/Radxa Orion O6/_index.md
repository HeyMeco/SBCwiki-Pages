---
weight: 1
title: Radxa Orion O6
categories:
- board
tags: 
- CD8180
boards:
- Orion-O6
board-vendor:
- Radxa
summary: "Radxa Orion O6 on SBCwiki.com"
images:
- images/spec_orion_o6_01.webp
---

# Radxa Orion O6

## Board Pictures
{{< gallery match="images/*" sortOrder="asc" rowHeight="150" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=true previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware
{{% details title="Specs" open=true %}}

| **SoC** | **CD8180 / P1**                                                                                                                  |
|---------|----------------------------------------------------------------------------------------------------------------------------------|
| **CPU** | 4x Cortex®-A720 (Big cores) up to 2.8GHz<br>4x Cortex®‑A720 (Medium cores) up to 2.4GHz<br>4x Cortex®‑A520 (LITTLE cores) 1.8GHz |
| **RAM** | LPDDR5 RAM<br>- 128bit memory bus<br>- 5500MT/s transfer speed<br>- Configurations: 4GB / 8GB / 16GB / 32GB / 64GB               |
| **GPU** | Arm® Immortalis™ G720 MC10<br>- Hardware Ray‑Tracing enabled<br>- Vulkan® 1.3<br>- OpenGL® ES 3.2<br>- OpenCL® 3.0               |
| **VPU** | – 8K@60fps decoder AV1, H.265, H.264, VP9, VP8, H.263, MPEG‑4, MPEG‑2<br>- 8K@30fps encoder H.265, H.264, VP9, VP8               |
| **NPU** | Neural Processing Unit (NPU)<br>- Computing Power: 30 TOPs<br>- Precision Support: INT4 / INT8 / INT16 / FP16 / TF32             |

---
### Interfaces

| **I/O**      | Description                                                                                                                                                                                                                                                             |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Wireless** | 1x M.2 E Key Connector with PCIe Gen4 2-lane and USB support for Wi-Fi7 & BT Module                                                                                                                                                                                     |
| **Ethernet** | 2x 5 Gigabit Ethernet Ports<br>- Speeds: 10 / 100 / 1000 / 2500 / 5000Mbps                                                                                                                                                                                              |
| **USB**      | 2x USB Type-C Ports<br>– Port 1: USB 3.2 Gen 2 (10Gbps) + Power Delivery<br>– Port 2: USB 3.2 Gen 2 (10Gbps) + DP Alt Mode (4K@60Hz) + Power Delivery<br>2x USB 3.2 HOST Type-A Ports(10Gbps)<br>2x USB 2.0 HOST Type-A Ports<br>2x USB 2.0 HOST via Front Panel Header |
| **Video**    | 2x USB Type-C Ports<br>– Port 1: USB 3.2 Gen 2 (10Gbps) + Power Delivery<br>– Port 2: USB 3.2 Gen 2 (10Gbps) + DP Alt Mode (4K@60Hz) + Power Delivery<br>2x USB 3.2 HOST Type-A Ports(10Gbps)<br>2x USB 2.0 HOST Type-A Ports<br>2x USB 2.0 HOST via Front Panel Header |
| **MicroSD**  | n/a                                                                                                                                                                                                                                                                     |
| **Storage**  | 1x M.2 M Key Connector with PCIe Gen4 4-lane support for M.2 M Key 2280 NVMe SSD                                                                                                                                                                                        |
| **Power**    | 1x 24-Pin ATX Power Supply Connector<br>- Standard Motherboard Power Input<br>- Compatible with ATX Power Supplies<br>1x USB Type-C Port with Power Delivery                                                                                                            |
| **GPIO**     | 40-pin header                                                                                                                                                                                                                                                           |
| **PCIe**     | PCIe x16 Physical Slot with PCIe Gen4 8-lane support<br>- Supports graphics cards, AI accelerator and other PCIe devices                                                                                                                                                |
| **MIPI**     | 2x MIPI Camera Interfaces<br>– Configurable as 4-lane or 2-lane MIPI CSI each                                                                                                                                                                                           |
| **RTC**      | powered from CR1220 battery                                                                                                                                                                                                                                             |

{{% /details %}}

## Available OS images
- Radxa official images
- All UEFI based ARM images (with Kernel 6.6 and above)

## Documentation / Links

- [Vendor Docs](https://docs.radxa.com/en/orion/o6)

## Benchmarks

- [GeekBench](https://browser.geekbench.com/v6/cpu/10409724) 6.4.0 Preview for Linux AArch64:<br> Single Core **1321**, Multi Core **6666**
- [Tkaiser's SBC-Bench](https://github.com/ThomasKaiser/sbc-bench/blob/master/results/reviews/Radxa-Orion-O6-1.0.md)

## Guides

- [Getting Started with Orion O6](https://docs.radxa.com/en/orion/o6/getting-started) 

## Articles

- [CNX-Software: Radxa Orion O6 Review](https://www.cnx-software.com/2025/01/29/radxa-orion-o6-review-unboxing-debian-12-installation-and-first-benchmarks/)