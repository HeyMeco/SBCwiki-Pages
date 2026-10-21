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

| **SoC** | **Qualcomm Dragonwing Q2 (QRB2210)** |
|:--- |:--- |
| **CPU** | 4x Arm Cortex-A53 @ 2.0 GHz |
| **GPU** | Qualcomm Adreno 702 @ 845 MHz |
| **ISP** | Dual ISP: 13 MP + 13 MP, or 25 MP @ 30 fps |
| **RAM** | LPDDR4X, 32-bit single-rank<br>- 2GB (ABX00162)<br>- 4GB (ABX00173) |
| **Storage** | eMMC 16GB (ABX00162) or 32GB (ABX00173) |

<br>

| **Microcontroller (MCU)** | **STM32U585** |
|:--- |:--- |
| **CPU** | Arm Cortex-M33 up to 160 MHz |
| **Flash** | 2MB |
| **RAM** | 786kB SRAM |
| **OS** | Arduino Core on Zephyr |

---
### Interfaces

| **I/O**      | Description                                                                                                                                                                                                                                                             |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Wireless** | Wi-Fi 5 dual-band (802.11a/b/g/n/ac) and Bluetooth 5.1<br>Onboard antenna (WCBN3536A / Qualcomm WCN3980)                                                                                                                                                                                                                      |
| **USB**      | 1x USB-C 3.1 with role switching<br>DisplayPort Alt Mode through an ANX7625 MIPI DSI-to-DisplayPort bridge                                                                                                                                                                                                                 |
| **Video**    | DisplayPort over USB-C<br>4-lane MIPI DSI on the JMEDIA connector                                                                                                                                                                                                                     |
| **Camera**   | 4-lane MIPI CSI-2 on the JMEDIA connector                                                                                                                                                                                                                                |
| **Power**    | USB-C Power Delivery, 5V / 3A only<br>7–24V DC on VIN<br>5V pin on the analog header                                                                                                                                                            |
| **GPIO**     | Arduino UNO headers (JDIGITAL, JANALOG) at 3.3V<br>JSPI header<br>Qwiic connector<br>JMEDIA 60-pin, 1.8V (MIPI CSI / DSI)<br>JMISC mixed-voltage header (1.8V MPU, 3.3V MCU)                                                                                                                                                                                                                              |
| **Other**    | 8×13 blue LED matrix driven by the STM32<br>RGB status LEDs<br>Uno form factor                                                                                                                                                                                                              |

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
