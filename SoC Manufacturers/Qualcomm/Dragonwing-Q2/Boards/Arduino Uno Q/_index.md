---
weight: 1
title: Arduino Uno Q
categories:
- board
tags: 
- QRB2210
boards:
- Arduino-Uno-Q
board-vendor:
- Arduino
summary: "Arduino Uno Q single-board computer - Qualcomm Dragonwing Q2 (QRB2210) quad Cortex-A53 running Debian, plus an STM32U585 Cortex-M33 for Arduino sketches, in the Uno form factor."
images:
- images/1-uno-q_top.webp
- images/2-uno-q_bottom.webp
---

# Arduino Uno Q

## Board Pictures
{{< gallery match="images/*" sortOrder="asc" rowHeight="150" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=true previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware
{{% details title="Specs" open=true %}}
{{< board-specs show="soc" >}}

### Microcontroller

{{< board-specs show="mcu" >}}

### Interfaces

{{< board-specs show="board" >}}
{{% /details %}}

## Available OS images
- Debian, from Arduino, with upstream Linux support on the QRB2210
- Arduino App Lab, bridging Linux on the QRB2210 and sketches on the STM32U585

## Documentation / Links

- [Arduino UNO Q documentation](https://docs.arduino.cc/hardware/uno-q)
- [Datasheet](https://docs.arduino.cc/resources/datasheets/ABX00162-datasheet.pdf)
- [Product page](https://www.arduino.cc/product-uno-q)

## Benchmarks

- Geekbench 6, from sbc.compare:<br> Single Core **190**, Multi Core **527**

## Guides

- [UNO Q power specifications](https://docs.arduino.cc/tutorials/uno-q/power-specification/)
