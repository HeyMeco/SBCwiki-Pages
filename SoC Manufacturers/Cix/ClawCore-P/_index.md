---
weight: 2
title: "Cix ClawCore-P: Specs, Features and AI Performance"
linktitle: "ClawCore-P"
soc-series:
- ClawCore
soc:
- ClawCore-P
tags:
- SOC-Cix
summary: Cix ClawCore-P (勁螯芯) — 12-core Armv9.2 SoC with Immortalis-G720 GPU, 45 TOPS AI, up to 64GB LPDDR5, optimized for OpenClaw deployments.
---
# Cix ClawCore-P

**ClawCore-P** (勁螯芯, “Powerful Claw”) is the high-performance SKU in Cix’s **ClawCore** Armv9.2 CPU family, marketed for [OpenClaw](https://www.openclaw.ai/) agent workloads and high-parallelism, large-memory scenarios.

Specifications are close to the [Cix P1 (CD8180)]({{< relref "/docs/SoC Manufacturers/Cix/CD8180-P1" >}}) (12 Armv9.2-class cores, Immortalis-G720, large LPDDR5 capacity), with a higher advertised CPU clock (up to 3.2 GHz). Combined AI compute is quoted at **45 TOPS**. Mini PCs and workstations based on ClawCore-P were expected to ship from **March 2026**.

## General specifications
{{% details title="Specs" open=true %}}

| **Product** | **ClawCore-P** |
|-------------|----------------|
| **CPU** | 12-core Armv9.2 @ up to 3.2 GHz |
| **RAM** | Up to 64 GB LPDDR5 |
| **GPU** | Arm Immortalis-G720 |
| **AI** | ~45 TOPS combined (vendor figure) |
| **Target** | OpenClaw, high parallelism, large-capacity local inference |

{{% /details %}}

---

## Software and platform

Cix positions ClawCore alongside software support that includes an **Open AI Agent Hub** for shared models and skills, integrated OpenClaw-oriented delivery, multi-system agent collaboration, hardware-backed security, and power tuning for always-on systems. Developers get an SDK; platforms are aimed at **Arm SystemReady**-class support with **Windows**, **Android**, **Ubuntu**, **UnionTech UOS / Tongxin**, and **Kylin** called out in press coverage.

---

## Boards

Systems from partners such as Orange Pi (Xunlong), Radxa, and others are expected over time.

{{< taglist tag="ClawCore-P" style="cards" >}}

## FAQ: Cix ClawCore-P

{{% columns %}}
- {{< card title="What is the Cix ClawCore-P?" >}}
  The Cix ClawCore-P is a high-performance 12-core Armv9.2 SoC featuring an Immortalis-G720 GPU and up to 64GB of LPDDR5 RAM, optimized for OpenClaw agent workloads.
  {{< /card >}}

- {{< card title="How much AI compute does the ClawCore-P have?" >}}
  The ClawCore-P offers approximately 45 TOPS of combined AI compute performance for local inference and high-parallelism tasks.
  {{< /card >}}
{{% /columns %}}

{{% columns %}}
- {{< card title="What operating systems are supported on ClawCore-P?" >}}
  It targets Arm SystemReady-class support, with compatibility for Windows, Android, Ubuntu, UnionTech UOS, and Kylin.
  {{< /card >}}

- {{< card title="When are ClawCore-P boards shipping?" >}}
  Mini PCs and workstations based on the ClawCore-P, including systems from partners like Orange Pi and Radxa, were expected to ship starting from March 2026.
  {{< /card >}}
{{% /columns %}}
