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

> **Note:** From 2025, ARM uses the **C1** branding (C1-Ultra, C1-Premium, C1-Pro, C1-Nano) instead of "Cortex" for the new CPU line.

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

> Neoverse targets datacenter and infrastructure; Cortex-A/X target mobile and client.

### 2018

| ISA | Name | Class |
|-----|------|-------|
| ARMv8.2-A | Cortex-A76 | Performance |
| ARMv8.2-A | Cortex-A76AE | Performance (Safety) |
| ARMv8.2-A | Cortex-A65 | Performance |
| ARMv8.2-A | Cortex-A65AE | Performance (Safety) |

 > AE variants add safety features (e.g. lockstep) commonly used in Automotive.

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
