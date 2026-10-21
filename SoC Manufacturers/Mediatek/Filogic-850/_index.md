---
weight: 12
title: Filogic 850
soc-series:
- Filogic
soc:
- Filogic-850
tags:
- SOC-MTK-Router
summary: MediaTek Filogic 850 cost-effective Wi-Fi 7 AP SoC — quad Cortex-A53 @ 2 GHz, BE3600 dual-band Wi-Fi 7, NPU offload, 2.5 GbE and 1 GbE.
---
# Filogic 850

The MediaTek Filogic 850 is the cost-effective Wi-Fi 7 AP and CPE platform in the Filogic line. It pairs a quad-core Cortex-A53 CPU at 2 GHz with dual-band Wi-Fi 7 up to BE3600, a dedicated networking NPU, and multi-gig Ethernet options for routers, repeaters, gateways, and access points.

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **Filogic 850** |
|---------|-----------------|
| **CPU** | 4× Arm Cortex-A53 @ 2 GHz (about 18.4K DMIPS) |
| **RAM** | Up to DDR4-3200 |
| **Wi-Fi** | Dual-band Wi-Fi 7 (a/b/g/n/ac/ax/be)<br>Up to 3.6 Gbps (BE3600)<br>2.4 GHz 2T2R 2SS, 5 GHz 3T3R 2SS / 2T2R+1R 0-DFS<br>4096-QAM, single-MAC MLO, Multi-RU |
| **Ethernet** | 2× 2.5 GbE via HSGMII, built-in 1 GbE PHY |
| **NPU** | Up to 7.5 Gbps packet processing<br>800 Kpps Wi-Fi offload<br>HW acceleration for PPPoE, VLAN, MAP-E, DS-Lite |
| **Security** | Secure Boot, Arm TrustZone, EIP-197 crypto, FIPS 140-3 support |
| **I/O** | PCIe 3.0 (2x1 or 1x2), USB 3.2 Gen1 (shared with HSGMII), SPI, I2C, UART, GPIO, PCM/I2S |

{{% /details %}}

### Variant Differences:

- **Filogic 850**: Mainstream cost-down Wi-Fi 7 platform versus Filogic 860/880. Integrated iFEM (PA and LNA) in the MediaTek RFIC for both bands to shrink BOM size.

---

## Linux Support

### Mainline / OpenWrt

- Filogic 850 is part of MediaTek's Wi-Fi 7 Filogic family. Board support depends on the specific OEM design and OpenWrt target coverage for that SKU.

---

## Resources

- [Filogic 850 product page](https://www.mediatek.com/products/broadband-wifi/mediatek-filogic-850)

---

## Boards with Filogic 850

List of boards:

{{< taglist tag="Filogic-850" style="cards" >}}
