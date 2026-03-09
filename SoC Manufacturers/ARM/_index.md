---
weight: 1
title: ARM
icon: /assets/arm/Arm_Logo.png
iconBg: "#098DAD"
categories:
- soc-vendors
soc-vendors:
- ARM
bookCollapseSection: true
summary: All ARM CPU cores & GPUs and other resources on sbcwiki.com
bookToc: true
---
<style>
/* On this page only: hide H3+ in all TOC variants */
.book-toc nav ul ul,      /* desktop sidebar */
.book-header nav ul ul {  /* inline header TOC */
  display: none;
}

/* On this page only: make all tables use equal column widths */
.markdown table {
  width: 100%;
  table-layout: fixed;
}
.markdown table th,
.markdown table td {
  width: 33.3333%;
}
</style>

![ARM Logo](assets/arm/Arm_Logo.png?h=100&bc=098DAD)

## Summary

Arm Holdings is a semiconductor and software design company based in Cambridge, England, whose primary business is the design of central processing unit (CPU) cores that implement the ARM architecture family of instruction sets. They also design their own GPUs called Mali / Immortalis as well as NPUs called Ethos.

## ARM CPU Cores

All ARMv8-A and newer cores

### 2025

| ISA | Name | Class |
|-----|------|-------|
| ARMv9.3-A | C1-Ultra (Cortex-X930) | Flagship |
| ARMv9.3-A | C1-Premium (Cortex-A730) | High-End |
| ARMv9.3-A | C1-Pro (Cortex-A530) | Performance |
| ARMv9.3-A | C1-Nano (Cortex-A320) | Ultra Efficiency |

### 2024

| ISA | Name | Class |
|-----|------|-------|
| ARMv9.2-A | Cortex-X925 | Flagship |
| ARMv9.2-A | Cortex-A725 | High-End |
| ARMv9.2-A | Cortex-A720AE | Performance |
| ARMv9.2-A | Cortex-A520AE | Efficiency |
| ARMv8-R | Cortex-R82AE | Real-Time |

### 2023

| ISA | Name | Class |
|-----|------|-------|
| ARMv9.2-A | Cortex-X4 | Flagship |
| ARMv9.2-A | Cortex-A720 | Performance |
| ARMv9.2-A | Cortex-A520 | Efficiency |
| ARMv9.2-A | Neoverse N3 (Cortex-X3) | Infrastructure |
| ARMv9.2-A | Neoverse V3 (Cortex-X4) | Infrastructure |

### 2022

| ISA | Name | Class |
|-----|------|-------|
| ARMv9.0-A | Cortex-X3 | Flagship |
| ARMv9.0-A | Cortex-A715 | Performance |
| ARMv9.0-A | Neoverse V2 (Cortex-X2) | Infrastructure |
| ARMv8-R | Cortex-R52+ | Real-Time |
| ARMv8.2-A | Cortex-M85 | Microcontroller |

### 2021

| ISA | Name | Class |
|-----|------|-------|
| ARMv9.0-A | Cortex-X2 | Flagship |
| ARMv9.0-A | Cortex-A710 | Performance |
| ARMv9.0-A | Cortex-A510 | Efficiency |
| ARMv9.0-A | Neoverse N2 (Cortex-A710) | Infrastructure |
| ARMv9.0-A | Neoverse E2 (Cortex-A510) | Infrastructure |

### 2020

| ISA | Name | Class |
|-----|------|-------|
| ARMv8.2-A | Cortex-X1 | Flagship |
| ARMv8.2-A | Cortex-A78 | Performance |
| ARMv8.2-A | Cortex-A78AE | Performance (Safety) |
| ARMv8.2-A | Cortex-A78C | Performance |
| ARMv8.4-A | Neoverse V1 (Cortex-X1) | Infrastructure |
| ARMv8-R | Cortex-R82 | Real-Time |

### 2019

| ISA | Name | Class |
|-----|------|-------|
| ARMv8.2-A | Cortex-A77 | Performance |
| ARMv8-A | Cortex-A34 | Ultra Efficiency |
| ARMv8.2-A | Neoverse N1 (Cortex-A76) | Infrastructure |
| ARMv8.2-A | Neoverse E1 (Cortex-A75) | Infrastructure |

### 2018

| ISA | Name | Class |
|-----|------|-------|
| ARMv8.2-A | Cortex-A76 | Performance |
| ARMv8.2-A | Cortex-A76AE | Performance (Safety) |
| ARMv8.2-A | Cortex-A65 | Performance |
| ARMv8.2-A | Cortex-A65AE | Performance (Safety) |

### 2017

| ISA | Name | Class |
|-----|------|-------|
| ARMv8.2-A | Cortex-A75 | Performance |
| ARMv8.2-A | Cortex-A55 | Efficiency |

### 2016

| ISA | Name | Class |
|-----|------|-------|
| ARMv8-A | Cortex-A73 | Performance |
| ARMv8-A | Cortex-A32 | Ultra Efficiency (32-bit) |

### 2015

| ISA | Name | Class |
|-----|------|-------|
| ARMv8-A | Cortex-A72 | Performance |
| ARMv8-A | Cortex-A35 | Ultra Efficiency |

### 2012

| ISA | Name | Class |
|-----|------|-------|
| ARMv8-A | Cortex-A57 | Performance |
| ARMv8-A | Cortex-A53 | Efficiency |

> **Note:** From 2025, ARM uses the **C1** branding (C1-Ultra, C1-Premium, C1-Pro, C1-Nano) instead of "Cortex" for the new CPU line. AE variants add safety features (e.g. lockstep) commonly used in Automotive. Neoverse targets datacenter and infrastructure; Cortex-A/X target mobile and client.

## ARM Mali GPUs

### 2025

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Magni "5th Gen" (v14) | Mali G1-Ultra | Flagship |
| Magni "5th Gen" (v14) | Mali G1-Premium | Mid-Range |
| Magni "5th Gen" (v14) | Mali G1-Pro | Entry |

### 2024

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| 5th Gen (v13) | Immortalis-G925 | Flagship |
| 5th Gen (v13) | Mali-G725 | Mid-Range |
| 5th Gen (v13) | Mali-G625 | Entry |

### 2023

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| 5th Gen (v12) | Immortalis-G720 | Flagship |
| 5th Gen (v12) | Mali-G720 | Sub-Premium |
| 5th Gen (v12) | Mali-G620 | Mid-Range |

### 2022

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Valhall (v11) | Immortalis-G715 | Flagship |
| Valhall (v11) | Mali-G715 | Sub-Premium |
| Valhall (v11) | Mali-G615 | Mid-Range |

> **Note:** Immortalis (G715, G720, G925) share the same architecture version as their Mali siblings (v11, v12, v13); the Linux kernel distinguishes them by **10+ shader cores** and **hardware ray intersection** support, not by a different arch version. Utgard-based GPUs are supported by the Lima driver; Midgard and newer are supported by Panfrost/Panthor.
> <br>**Source**: [Linux Kernel - Panthor_hw.c](https://github.com/torvalds/linux/blob/master/drivers/gpu/drm/panthor/panthor_hw.c)

### 2021

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Valhall (v10) | Mali-G710 | High-End |
| Valhall (v10) | Mali-G610 | Sub-Premium |
| Valhall (v10) | Mali-G510 | Mid-Range |
| Valhall (v10) | Mali-G310 | Entry |

### 2020

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Valhall (v9) | Mali-G78 | High-End |
| Valhall (v9) | Mali-G68 | Mid-Range |
| Valhall (v9) | Mali-G78AE | Automotive |

### 2019

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Valhall (v9) | Mali-G77 | High-End |
| Valhall (v9) | Mali-G57 | Mid-Range |

### 2018

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Bifrost (v7) | Mali-G76 | High-End |
| Bifrost (v7) | Mali-G52 | Mid-Range |
| Bifrost (v7) | Mali-G31 | Entry |

### 2017

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Bifrost (v6) | Mali-G72 | High-End |

### 2016

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Bifrost (v6) | Mali-G71 | High-End |
| Midgard (v5) | Mali-T880 | High-End |
| Bifrost (v6) | Mali-G51 | Mid-Range |

### 2015

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Midgard (v5) | Mali-T860 | High-End |
| Midgard (v5) | Mali-T830 | Mid-Range |
| Utgard | Mali-470 | Mid-Range |
| Midgard (v5) | Mali-T820 | Entry |

### 2013

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Midgard (v5) | Mali-T760 | High-End |
| Midgard (v4) | Mali-T720 | Mid-Range |
| Midgard (v4) | Mali-T622 | Entry |

### 2012

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Midgard (v4) | Mali-T678 | High-End |
| Midgard (v4) | Mali-T628 | High-End |
| Midgard (v4) | Mali-T624 | Mid-Range |
| Utgard | Mali-450 | Mid-Range |

### 2011

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Midgard (v4) | Mali-T658 | High-End |

### 2010

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Midgard (v4) | Mali-T604 | High-End |
| Utgard | Mali-300 | Entry |

### 2008

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Utgard | Mali-400 | Entry |

### 2007

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Utgard | Mali-200 | Entry |

### 2005

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| Utgard | Mali-55 / Mali-110 | Entry |
