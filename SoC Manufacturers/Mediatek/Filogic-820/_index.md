---
weight: 13
title: Filogic 820 / MT7981
soc-series:
- Filogic
soc:
- Filogic-820
- MT7981
tags:
- SOC-MTK-Router
summary: MediaTek Filogic 820 (MT7981) entry Wi-Fi 6 router SoC — dual Cortex-A53 @ 1.3 GHz, 2.5 GbE + 1 GbE, used on the OpenWrt One.
---
# Filogic 820 / MT7981

The MediaTek Filogic 820 is the entry Wi-Fi 6 SoC in the Filogic line. The silicon is **MT7981** / **MT7981B**: dual Cortex-A53 cores at 1.3 GHz, with 2.5 GbE and 1 GbE networking and a companion Wi-Fi 6 radio such as the MT7976C. It is the chip on the official **OpenWrt One** reference router.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

<br>
{{% details title="OpenWrt One reference" open=false %}}

The OpenWrt One pairs MT7981B with 1 GB DDR4, dual flash (SPI-NAND + SPI-NOR) for recovery, 2.5 GbE + 1 GbE, MT7976C Wi-Fi 6, M.2 NVMe, and a MikroBUS expansion socket.

{{% /details %}}

### Variant Differences:

- **MT7981 / MT7981B**: Dual-core Filogic 820. Common on AX3000-class routers (Xiaomi AX3000T, GL.iNet GL-MT3000, Cudy WR3000, and others) and the OpenWrt One.
- **MT7986 / Filogic 830**: Related higher-tier Wi-Fi 6 SoC with four Cortex-A53 cores; not listed separately on this page.

---

## Linux Support

### Mainline / OpenWrt

- [x] Fully supported in OpenWrt `mediatek/filogic`
- [x] OpenWrt One is an official OpenWrt project board

---

## Resources

- [OpenWrt One (Banana Pi docs)](https://docs.banana-pi.org/en/OpenWRT-One/BananaPi_OpenWRT-One)
- [OpenWrt mediatek/filogic target](https://openwrt.org/docs/techref/hardware/soc/soc.mediatek)

---

## Boards with Filogic 820

List of boards:

{{< taglist tag="Filogic-820" style="cards" >}}

{{< taglist tag="MT7981" style="cards" >}}
