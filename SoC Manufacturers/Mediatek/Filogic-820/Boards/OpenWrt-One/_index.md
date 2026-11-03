---
weight: 1
title: OpenWrt One
categories:
- board
tags:
- Filogic-820
- MT7981
boards:
- OpenWrt-One
board-vendor:
- OpenWrt
- BananaPi
release: "2024-11"
summary: "OpenWrt One router board - MediaTek MT7981B dual Cortex-A53, 1 GB DDR4, 2.5 GbE + 1 GbE, Wi-Fi 6, NAND + write-protected NOR recovery, M.2 NVMe."
---
# OpenWrt One

The OpenWrt One is the OpenWrt project's own reference router. The OpenWrt project designed it, and Banana Pi manufactures and sells it. It is built to be hard to brick. The bootloader and Linux live on SPI NAND, while a write-protected SPI NOR holds a recovery system. A switch picks which one the board boots from. Mainline Linux device-tree support is being upstreamed.

## Hardware
{{% details title="Specs" open=true %}}
{{< board-specs show="soc" >}}

### Interfaces

{{< board-specs show="board" >}}
{{% /details %}}

## Available OS images

{{< list-board-available-os >}}

## Documentation / Links

- [OpenWrt One (OpenWrt wiki)](https://openwrt.org/toh/openwrt/one)
- [OpenWrt One (Banana Pi docs)](https://docs.banana-pi.org/en/OpenWRT-One/BananaPi_OpenWRT-One)
- [Banana Pi forum: OpenWrt One](https://forum.banana-pi.org/t/openwrt-one-opensource-wifi6-router-with-mediatek-mt7981b-chip/18168)

## Benchmarks

## Guides

## Articles
