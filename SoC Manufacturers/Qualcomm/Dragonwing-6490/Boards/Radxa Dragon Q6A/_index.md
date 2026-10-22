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
summary: "Radxa Dragon Q6A single-board computer - QCS6490 8-core ARM processor, up to 32GB LPDDR5, Adreno 643 GPU, M.2 NVMe, WiFi 6E, Bluetooth 5.2."
images:
- images/1-q6a_top.webp
---

# Radxa Dragon Q6A

## Board Pictures
{{< gallery match="images/*" sortOrder="asc" rowHeight="150" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=true previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware
{{% details title="Specs" open=true %}}
{{< board-specs show="soc" >}}

### Interfaces

{{< board-specs show="board" >}}
{{% /details %}}

## Available OS images
- Radxa official images
- Windows 11 on Arm
  - Drivers supplied from vendor [here](https://forum.radxa.com/t/windows-on-radxa-dragon-q6a/29913?u=meco) not Qualcomm
  - Boots regular ARM ISO's from Microsoft (LTSC and other versions possible)
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

- [SBCwiki - Radxa Dragon Q6A First-Look](/news/articles/radxa-dragon-q6a-unboxing-and-first-look/)
- [SBCwiki - Radxa Dragon Q6A Full Review](/news/articles/radxa-dragon-q6a-full-review/)
- [Anton Maltsev - Radxa Dragon Q6A for Edge AI](https://medium.com/@zlodeibaal/inside-the-radxa-dragon-q6a-a-deep-dive-into-qualcomms-new-edge-ai-platform-34b61a4f2918)