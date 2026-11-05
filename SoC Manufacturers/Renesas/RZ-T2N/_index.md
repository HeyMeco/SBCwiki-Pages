---
weight: 10
title: Renesas RZ/T2N
soc-series:
- RZ-T
soc:
- RZ-T2N
tags:
- SOC-Renesas
- RZ-T2N
summary: Renesas RZ/T2N industrial MPU - dual Cortex-A55 (1.2 GHz) and dual Cortex-R52 (800 MHz), 4-axis motor control, 3× Gigabit Ethernet with switch, EtherCAT and TSN, and 16-bit LPDDR4-1600 with ECC.
---
# Renesas RZ/T2N

The RZ/T2N is a 64-bit industrial MPU for robots and multi-axis motion control, announced on 5 November 2026. Two Cortex-A55 cores run Linux and the application. Two Cortex-R52 cores handle real-time control, each with 576 KB of TCM with ECC. Renesas showed it at electronica 2026 in Munich, 10–13 November (Hall C5, Stand 479).

- **Motor control:** peripherals for up to 4 axes, with 2 encoder channels per axis. Supported encoder protocols are Tamagawa T-Format, HIPERFACE DSL, A-format, EnDat 2.2, EnDat 3, BiSS C and BiSS Line.
- **Industrial Ethernet:** 3 Gigabit Ethernet MACs, an Ethernet switch and an EtherCAT SubDevice Controller (ESC). It supports EtherCAT, PROFINET RT/IRT, EtherNet/IP and TSN, with HSR/PRP/FRER redundancy.
- **Safety and security:** ECC on TCM, cache, on-chip SRAM and DDR, and on-the-fly DDR encryption and decryption. It also has a crypto library, secure boot, secure firmware update and Arm TrustZone.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

---

## Linux Support

### Vendor BSP
- Renesas ships one Linux package and its Flexible Software Package (FSP) for the whole RZ/T2x and RZ/N2x range
- An evaluation board is available from Renesas

### Mainline kernel
- [ ] Fully supported
- [ ] Works but not all features are implemented.
- Unknown, not checked yet

---

## Documentation

- [RZ/T2N product page](https://www.renesas.com/rzt2n)
- [RZ/T2N announcement (press release)](https://www.renesas.com/en/about/newsroom/new-rzt2n-mpu-integrates-motor-control-industrial-ethernet-and-application-processing-robots-and)

---

## Boards with Renesas RZ/T2N

{{< taglist tag="RZ-T2N" style="cards" >}}
