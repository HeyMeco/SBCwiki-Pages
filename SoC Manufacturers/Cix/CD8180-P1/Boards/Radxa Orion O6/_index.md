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
{{< board-specs show="soc" >}}

### Interfaces

{{< board-specs show="board" >}}
{{% /details %}}

## Available OS images
- Radxa Debian image (BSP Kernel, supports Device Tree & ACPI)
- Radxa Android 14 image
- All UEFI based ARM images (with Mainline Kernel 6.6 and above)

## Documentation / Links

- [Vendor Docs](https://docs.radxa.com/en/orion/o6)

## Benchmarks

- [GeekBench](https://browser.geekbench.com/v6/cpu/10409724) 6.4.0 Preview for Linux AArch64:<br> Single Core **1321**, Multi Core **6666**
- [Tkaiser's SBC-Bench](https://github.com/ThomasKaiser/sbc-bench/blob/master/results/reviews/Radxa-Orion-O6-1.0.md)

## Guides

- [Getting Started with Orion O6](https://docs.radxa.com/en/orion/o6/getting-started) 

## Articles

- [CNX-Software: Radxa Orion O6 Review](https://www.cnx-software.com/2025/01/29/radxa-orion-o6-review-unboxing-debian-12-installation-and-first-benchmarks/)