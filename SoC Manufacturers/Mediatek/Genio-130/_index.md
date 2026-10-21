---
weight: 6
title: Genio 130 / MT7933
soc-series:
- Genio
soc:
- Genio-130
- Genio-130A
- MT7933
- MT7931
tags:
- SOC-MTK
summary: MediaTek Genio 130 / 130A (MT7931 / MT7933) Cortex-M33 IoT MCU with Wi-Fi 6, Bluetooth 5.2, HiFi 4 DSP, and Matter-ready SDK options.
---
# Genio 130 / MT7933

The MediaTek Genio 130 family is the MCU tier of Genio. It is not an application-processor Linux SoC. The silicon is a Cortex-M33 with integrated dual-band Wi-Fi 6, Bluetooth, and a HiFi 4 audio DSP, aimed at smart home, Matter, and voice devices. Genio 130A is the MT7933CT SKU with USB 2.0 OTG and the HiFi 4 DSP enabled.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **MediaTek Genio 130A / MT7933CT** |
|---------|-------------------------------------|
| **CPU** | Arm Cortex-M33 with FPU<br>Up to 300 MHz (0.8 V), 200 MHz at 0.7 V |
| **Memory** | 1 MB SRAM<br>8 MB UHS PSRAM<br>Up to 96 KB TCM/cache<br>External serial flash with XIP and on-the-fly AES |
| **Audio DSP** | Cadence Tensilica HiFi 4 @ up to 600 MHz (MT7933) |
| **Wi-Fi** | 802.11a/b/g/n/ac/ax 1T1R dual-band<br>20 MHz, MU-OFDMA, WPA3 |
| **Bluetooth** | Bluetooth 5.2 |
| **Security** | AES, DES/3DES, SHA, ECC, TRNG |
| **I/O** | USB 2.0 OTG (MT7933), SDIO, SPI master/slave, I2C, I2S, UART, AUXADC, PWM<br>Up to about 47 GPIOs |
| **Package** | 10.6 × 10.6 mm BGA |
| **Power** | Single 3.3 V input with integrated PMU |

{{% /details %}}

### Variant Differences:

- **Genio 130A / MT7933**: Full SKU with HiFi 4 DSP and USB 2.0 OTG. FreeRTOS and Arduino SDKs. Matter examples exist in community and partner solutions.
- **Genio 130 / MT7931**: Related part in the same family with a reduced feature set versus MT7933 (no HiFi 4 / USB 2.0 on the lighter SKUs).

---

## Linux Support

### Mainline kernel

- Not applicable as a Linux application processor. Firmware targets FreeRTOS and Arduino-style SDKs.

---

## Resources

- [MT7933CT datasheet (MediaTek)](https://www.mediatek.com/hubfs/MediaTek%20Assets/Pdfs/Genio%20Documents/MT7933CT_Datasheet.pdf)
- [Genio IoT portfolio](https://www.mediatek.com/products/iot/genio-iot)

---

## Boards with Genio 130

List of boards:

{{< taglist tag="Genio-130" style="cards" >}}

{{< taglist tag="MT7933" style="cards" >}}
