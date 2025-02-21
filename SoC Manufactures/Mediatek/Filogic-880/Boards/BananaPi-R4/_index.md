---
weight: 1
title: BananaPi R4
categories:
- board
tags: 
- Filogic-880
boards:
- BananaPi-R4
---

# BananaPi R4

## Board Pictures
{{< gallery match="images/*" sortOrder="asc" rowHeight="150" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=true previewType="blur" embedPreview=true loadJQuery=true >}}

## Hardware
{{% details title="Specs" open=true %}}
Current Board Revision: 1.1

| **SoC** | **Filogic 880 / MT7988**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Quad-core ARM Cortex-A73 (up to 1.8GHz)                                                         |
| **RAM** | 4GB DDR4                                                                                                         |
| **GPU** | n/a                                                                                                            |
| **NPU** | HW IPv4 NATP / IPv6 / DS-Lite / 6RD acceleration <br> Hardware QoS acceleration <br> Tunneling Offload Engine for: <br> VLAN / PPTP / L2TP / GRE <br> Ultra-high Speed Networking Crypto Engine for: <br> IPSec,SSL/TLS, DTLS (CAPWAP), SRTP and MACsec                                                                       |
---
### Interfaces

| **I/O**      	| Description                                                                                                                                                          	|
|--------------	|----------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| **Wireless** 	| 2x miniPCIe slots with PCIe3.0 2-lane interface for Wi-Fi 7 NIC                                                                                                        |
| **Ethernet** 	| 2x 10Gbe SFP slot <br> 4x GbE network port                                                                                                                         	|
| **USB**      	| 1x USB3.2 slot                                                                                            	|
| **Video**    	| n/a 	|
| **MicroSD**  	| yes                                                                                                                                            	|
| **Storage**   | 8GB EMMC <br> 128MB SPI NAND Flash                                                                                                            |
| **Power**    	| USB Type‑C™ PD Version 2.0 with up to PD 20V <br> 12V/5.2A DC input (5521)                                                                                             	|
| **GPIO**     	| 26-pin header                                                                                                                                  	|
| **PCIe**     	| 1x M.2 KEY-M slot with PCIe3.0 1lane interface for NVME SSD <br> 1x M.2 KEY-B slot with USB3.2/PCIe3.0 interface for 5G                                                                                 	|
| **MIPI**     	| n/a                                                                                                                  	|
| **RTC**      	| powered from external battery                                                                                                                                        	|

{{% /details %}}

## Available OS images
- OpenWRT Snapshots at [OpenWRT Firmware Selector](https://firmware-selector.openwrt.org/?version=SNAPSHOT&target=mediatek%2Ffilogic&id=bananapi_bpi-r4)
{{< list-board-available-os >}}

## Documentation / Links

- [Vendor Wiki for BPI-R4](https://wiki.banana-pi.org/Banana_Pi_BPI-R4)
- [OpenWRT Wiki for BPI-R4](https://openwrt.org/inbox/toh/sinovoip/bananapi_bpi-r4)

## Benchmarks

- [Geekbench](https://browser.geekbench.com/v6/cpu/7137136) 6.3.0 Preview for Linux AArch64:<br> Single Core **302**, Multi Core **854**
## Guides

- [Getting Started with BPI-R4](https://wiki.banana-pi.org/Getting_Started_with_BPI-R4) 

## Articles

- [BPI-R4 by Frank Wunderlich](https://www.fw-web.de/dokuwiki/doku.php?id=en:bpi-r4:start)