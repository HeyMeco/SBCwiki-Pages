---
weight: 11
title: Filogic 860 / MT7987
soc-series:
- Filogic
soc:
- Filogic-860
- MT7987
tags:
- SOC-MTK-Router
summary: MediaTek Filogic 860 (MT7987) mainstream Wi-Fi 7 router SoC — quad Cortex-A53 up to 2.0 GHz in OpenWrt silicon, BE7200-class Wi-Fi 7 platform, multi-gig Ethernet.
---
# Filogic 860 / MT7987

The MediaTek Filogic 860 is the mainstream Wi-Fi 7 router and gateway platform below Filogic 880. OpenWrt and shipping boards identify the silicon as **MT7987** / **MT7987A**, with four Cortex-A53 cores up to 2.0 GHz. MediaTek markets the Filogic 860 platform for BE7200 dual-band Wi-Fi 7 APs, routers, and gateways with multi-gig Ethernet and a dedicated networking NPU.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

### Variant Differences:

- **MT7987A**: Quad Cortex-A53 @ 2.0 GHz. Used on boards such as the Banana Pi R4 Lite and GL.iNet MT5000. OpenWrt support landed in late 2025; WED/WO wireless offload still needs more work.
- **Filogic 860 platform**: MediaTek's product page emphasizes single-MAC MLO, BE7200 PHY, and multi-gig wired options for AP, router, repeater, and gateway designs.

---

## Linux Support

### Mainline / OpenWrt

- [x] OpenWrt `mediatek/filogic` target includes MT7987
- [ ] Wireless offload (WED/WO) and some PHY firmware paths are incomplete on early support

See OpenWrt pull request [#20304](https://github.com/openwrt/openwrt/pull/20304) for the initial MT7987 bring-up.

---

## Resources

- [Filogic 860 product page](https://www.mediatek.com/products/broadband-wifi/mediatek-filogic-860)
- [OpenWrt MT7987 support PR](https://github.com/openwrt/openwrt/pull/20304)

---

## Boards with Filogic 860

List of boards:

{{< taglist tag="Filogic-860" style="cards" >}}

{{< taglist tag="MT7987" style="cards" >}}
