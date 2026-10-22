---
weight: 1
title: CD8180 / CD8160 / P1
#bookCollapseSection: true
soc-series:
- Filogic
soc:
- CD8180
- CD8160
tags: 
- SOC-Cix
summary: Cix CD8180/P1 - High-performance 12-core SoC with Immortalis G720 GPU and 30 TOPS NPU
---
# CD8180 / CD8160 / P1

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

>[!NOTE]
>Every Cix P1 has been limited up to 2.6GHz afterwards while the original target was 2.8GHz

{{% /details %}}
<br>
{{% details title="Block Diagram" open=false %}}

![P1 Block Diagram](images/Cix-P1-Blockdiagram.webp)

{{% /details %}}

---

## Linux Support

### Mainline kernel
- [ ] Fully supported.
- [x] Works but not all features are implemented.
- Driver support status available [here](https://github.com/cixtech/linux-mainline/wiki)

---

## Available OS
- [Ubuntu Concept](https://discourse.ubuntu.com/t/ubuntu-concept-goes-cix-p1/82213)
- Vendor Releases (see board page)

---

## Boards with Cix P1

List of boards:

{{< taglist tag="CD8180" style="cards" >}} 

- Minisforum MS-R1
- Radxa Orion O6N
- OrangePi 6 Plus
- MetaComputing ARM AI PC

---

## What variant is CD8160?

> “CD8160 was the silkscreen used in early mass production. As PC/server models entered production, all silkscreen numbers were standardized to C*8180. CD8160 is no longer supplied.”

Cix P1 variants like CD8160 are all the same SoC from different batches in production. There are **no differences**.
