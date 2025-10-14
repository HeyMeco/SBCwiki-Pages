---
weight: 1
title: Radxa Dragon Q6A
categories:
- board
tags: 
- QCS6490
boards:
- Dragon-Q6A
board-vendor:
- Radxa
summary: "Radxa Dragon Q6A on SBCwiki.com"
images:
- images/1-q6a_top.webp
---

# Radxa Dragon Q6A

## Board Pictures
{{< gallery match="images/*" sortOrder="asc" rowHeight="150" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=true previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware
{{% details title="Specs" open=true %}}

| **SoC** | **Qualcomm QCS6490**                                                                                                                      |
|---------|-------------------------------------------------------------------------------------------------------------------------------------------|
| **CPU** | 1x Kryo Gold Plus @2.7GHz<br>3x Kryo Gold @2.4GHz<br>4x Kryo Silver @1.9GHz                                                             |
| **RAM** | LPDDR5<br>- Configurations: 4GB / 6GB / 8GB / 12GB / 16GB                                                                                |
| **GPU** | Qualcomm® Adreno 643<br>- OpenGL ES 3.2<br>- Vulkan 1.3<br>- OpenCL 2.2<br>- DirectX 12                                                 |
| **AI**  | Hexagon DSP + Hexagon Tensor Accelerator<br>- Combined AI computing power: up to 12 TOPS                                                 |
| **VPU** | 4K@60fps decoding (H.264/H.265/VP9)<br>4K@30fps encoding (H.264/H.265)                          |

---
### Interfaces

| **I/O**      | Description                                                                                                                                                                                                                                                             |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Wireless** | Wi-Fi 6, Bluetooth 5.4 (requires external antenna)                                                                                                                                                                                                                      |
| **Ethernet** | 1x Gigabit Ethernet port (PoE support requires external PoE HAT)                                                                                                                                                                                                        |
| **USB**      | 1x USB 3.1 Type-A HOST / OTG<br>3x USB 2.0 Type-A HOST                                                                                                                                                                                                                 |
| **Video**    | 1x HDMI port (up to 4K@60Hz)<br>1x 4-lane MIPI DSI                                                                                                                                                                                                                     |
| **Camera**   | 1x 4-lane MIPI CSI<br>2x 2-lane MIPI CSI                                                                                                                                                                                                                                |
| **Audio**    | 3.5mm 4-segment headphone jack (supports microphone input)<br>Stereo output, can drive 32Ω headphones                                                                                                   |
| **Storage**  | Boot: 32MB QSPI Nor Flash<br>Expandable: MicroSD card / eMMC module / UFS module / M.2 M Key 2230 NVMe SSD                                                                                                                                                            |
| **Power**    | USB Type-C 12V power input<br>External 12V pin power input<br>PoE power supply (requires external PoE HAT)                                                                                                                                                            |
| **GPIO**     | 40-Pin GPIO Header (UART, SPI, I2C, etc.)                                                                                                                                                                                                                              |
| **Other**    | 1x 2-pin 1.25mm Fan Connector<br>Power button, EDL button                                                                                                                                                                                                              |

{{% /details %}}

## Available OS images
- Radxa official images
- [Armbian](https://www.armbian.com/radxa-dragon-q6a/)

## Documentation / Links

- [Vendor Docs](https://docs.radxa.com/en/dragon/q6a)

## Benchmarks

- [GeekBench](https://browser.geekbench.com/v6/cpu/13394263) 6.4.0 Preview for Linux AArch64:<br> Single Core **1194**, Multi Core **3334**
- [Tkaiser's SBC-Bench](https://github.com/ThomasKaiser/sbc-bench/blob/master/results/reviews/Radxa-Dragon-Q6A.md)
- [sbc.compare results](https://sbc.compare/47-radxa-dragon-q6a-6gb)

## Guides

- [Getting Started with Dragon Q6A](https://docs.radxa.com/en/dragon/q6a/getting-started) 

## Articles

- [SBCwiki - Radxa Dragon Q6A First-Look](https://sbcwiki.com/news/articles/radxa-dragon-q6a-unboxing-and-first-look/)