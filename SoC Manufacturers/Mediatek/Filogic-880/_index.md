---
weight: 1
title: Filogic 880 / MT7988
#bookCollapseSection: true
soc-series:
- Filogic
soc:
- Filogic-880
tags: 
- SOC-MTK-Router
summary: MediaTek Filogic 880 (MT7988) networking ARM processor - Quad-core Cortex-A73 up to 1.8GHz, hardware NAT acceleration, WiFi 7 ready, IPSec/SSL offload, tunneling support.
---
# Filogic 880 / MT7988

## General Specifications
{{% details title="Specs" open=true %}}

| **SoC** | **Filogic 880 / MT7988**                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------|
| **CPU** | Quad-core ARM Cortex-A73 (up to 1.8GHz)                                                         |
| **RAM** | DDR3/4                                                                                                         |
| **GPU** | n/a                                                                                                            |
| **NPU** | HW IPv4 NATP / IPv6 / DS-Lite / 6RD acceleration <br> Hardware QoS acceleration <br> Tunneling Offload Engine for: VLAN / PPTP / L2TP / GRE <br> Ultra-high Speed Networking Crypto Engine for: <br> IPSec,SSL/TLS, DTLS (CAPWAP), SRTP and MACsec                                                                       |

{{% /details %}}
<br>
{{% details title="Block Diagram" open=false %}}

![MT7988 Block Diagram](images/MT7988-Block-Diagram.png?f=webp)

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [ ] Fully supported
- [x] Works but not all features are implemented.

See [Mailing list](http://lore.kernel.org/lkml/?q=MT7988)


---

## Boards with Filogic 880

List of boards:

{{< taglist Filogic-880 >}}