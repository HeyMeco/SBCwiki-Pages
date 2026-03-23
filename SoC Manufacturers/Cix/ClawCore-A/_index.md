---
weight: 3
title: "Cix ClawCore-A: Specs, Features and AI Performance"
linktitle: "ClawCore-A"
soc-series:
- ClawCore
soc:
- ClawCore-A
tags:
- SOC-Cix
summary: Cix ClawCore-A (智螯芯) — octa-core Armv9.2 SoC with 80 TOPS AI (expandable via PCIe), ECC, and security features for 24/7 OpenClaw-style deployments.
---
# Cix ClawCore-A

**ClawCore-A** (智螯芯, “AI / Smart Claw”) is the mid-tier SKU in Cix’s **ClawCore** Armv9.2 family, focused on **24/7** operation, **full-chain ECC**, and **hardware security** (encryption and key management) for local and hybrid AI inference.

## General specifications
{{% details title="Specs" open=true %}}

| **Product** | **ClawCore-A** |
|-------------|----------------|
| **CPU** | Octa-core Armv9.2 @ up to 3.0 GHz |
| **RAM** | Up to 64 GB LPDDR5 |
| **AI** | ~80 TOPS on-chip; up to ~200 TOPS with vendor PCIe AI accelerator card (press figures) |
| **Reliability** | Full-chain ECC (as advertised) |
| **Security** | Hardware encryption / key management (as advertised) |
| **Target** | Always-on agents, local inference to reduce cloud token use |

{{% /details %}}

Press reporting describes a hybrid local/online model where most requests are handled on-device. Large models (e.g. on the order of tens to over 100B parameters) are mentioned only at a high level in marketing materials and should be treated as **claims** until independent details ship.

**Launch** was reported as planned for **June 2026**.

---

## Software and platform

Same broad platform story as the rest of ClawCore: OpenClaw-oriented integration, agent hub, collaboration features, security, and power optimization; **Arm SystemReady**-style targets and OS support including **Windows**, **Android**, **Ubuntu**, **UnionTech UOS / Tongxin**, and **Kylin** per Cix’s messaging summarized in the press.

---

## Boards

No public board pages on SBCwiki yet.

{{< taglist tag="ClawCore-A" style="cards" >}}

## FAQ: Cix ClawCore-A

{{% columns %}}
- {{< card title="What is the Cix ClawCore-A?" >}}
  The Cix ClawCore-A is a mid-tier Armv9.2 SoC designed for 24/7 operation, featuring full-chain ECC and hardware security for local and hybrid AI inference.
  {{< /card >}}

- {{< card title="How much AI performance does the ClawCore-A offer?" >}}
  It delivers approximately 80 TOPS of on-chip AI performance, which can be expanded up to 200 TOPS using vendor PCIe AI accelerator cards.
  {{< /card >}}
{{% /columns %}}

{{% columns %}}
- {{< card title="What operating systems does the ClawCore-A support?" >}}
  It targets Arm SystemReady compliance with support for Windows, Android, Ubuntu, UnionTech UOS, and Kylin.
  {{< /card >}}

- {{< card title="When is the ClawCore-A launching?" >}}
  The Cix ClawCore-A was reported to launch around June 2026.
  {{< /card >}}
{{% /columns %}}
