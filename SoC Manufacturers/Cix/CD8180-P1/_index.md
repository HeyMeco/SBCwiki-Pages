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

| **SoC** | **CD8180 / P1**                                                                                                                  |
|---------|----------------------------------------------------------------------------------------------------------------------------------|
| **CPU** | 4x Cortex®-A720 (Big cores) up to 2.8GHz<br>4x Cortex®‑A720 (Medium cores) up to 2.4GHz<br>4x Cortex®‑A520 (LITTLE cores) 1.8GHz |
| **RAM** | LPDDR5 RAM<br>- 128bit memory bus<br>- 5500MT/s transfer speed<br>- Configurations: 4GB / 8GB / 16GB / 32GB / 64GB               |
| **GPU** | Arm® Immortalis™ G720 MC10<br>- Hardware Ray‑Tracing enabled<br>- Vulkan® 1.3<br>- OpenGL® ES 3.2<br>- OpenCL® 3.0               |
| **VPU** | Arm-China Linlon V8<br>- 8K@60fps decoder AV1, H.265, H.264, VP9, VP8, H.263, MPEG‑4, MPEG‑2<br>- 8K@30fps encoder H.265, H.264, VP9, VP8               |
| **NPU** | Arm-China Zhouyi<br>- Computing Power: 30 TOPs<br>- Precision Support: INT4 / INT8 / INT16 / FP16 / TF32             |

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
- [ ] Fully supported
- [x] Works but not all features are implemented.

See [Mailing list](http://lore.kernel.org/lkml/?q=Cix+P1)
| Component                                                                                   | Status      |
|---------------------------------------------------------------------------------------------|-------------|
| [Basic DT](https://lore.kernel.org/all/20250721144500.302202-1-peter.chen@cixtech.com/)     | **Merged**  |
| [MAILBOX/UART/Clock](https://lore.kernel.org/all/20250721144500.302202-1-peter.chen@cixtech.com/) | **Merged**  |
| [I2C & I3C](https://lore.kernel.org/all/20250903084713.3221907-1-jun.guo@cixtech.com/)      | **Merged**  |
| [SPI](https://lore.kernel.org/r/20250919013118.853078-1-jun.guo@cixtech.com/)               | v6.19-rc1   |
| [Pinctrl](https://lore.kernel.org/all/20251021070410.3585997-1-gary.yang@cixtech.com/)      | v6.19-rc1   |
| [PCIe](https://lore.kernel.org/linux-pci/20251020042857.706786-1-hans.zhang@cixtech.com/)   | v6.19-rc1   |
| [HDA](https://lore.kernel.org/r/20251029093840.876483-4-joakim.zhang@cixtech.com/)          | Reviewing   |
| [Reset](https://lore.kernel.org/all/20251113075935.774359-1-gary.yang@cixtech.com/)         | Reviewing   |




---

## Boards with Cix P1

List of boards:

{{< taglist CD8180 >}} 

- Minisforum MS-R1
- Radxa Orion O6N
- OrangePi 6 Plus
- MetaComputing ARM AI PC

---

## What variant is CD8160?

> “CD8160 was the silkscreen used in early mass production. As PC/server models entered production, all silkscreen numbers were standardized to C*8180. CD8160 is no longer supplied.”

Cix P1 variants like CD8160 are all the same SoC from different batches in production. There are **no differences**.
