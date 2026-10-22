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
keywords: ["ARM", "ARM CPU cores", "ARM Mali GPUs", "Cortex", "Neoverse", "specifications", "data sheet", "datasheet", "SoC vendors"]
summary: Explore all ARM CPU cores, Mali GPUs, and custom silicon like the Arm AGI CPU. Find specifications, architectures, and resources on sbcwiki.com.
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

## [Arm Silicon](./ARM-Silicon)

While Arm primarily licenses CPU and GPU designs to other manufacturers, they started to produce their own silicon for specific datacenter and AI infrastructure applications starting in 2026.
{{< taglist SOC-ARM >}}

## ARM CPU Cores

All ARMv8-A and newer cores, plus the Cortex-M microcontroller cores used in SoCs on this wiki

### 2025

{{< generation-table "2025" >}}

> **Note:** From 2025, ARM uses the **C1** branding (C1-Ultra, C1-Premium, C1-Pro, C1-Nano) instead of "Cortex" for the new CPU line.

### 2024

{{< generation-table "2024" >}}

### 2023

{{< generation-table "2023" >}}

### 2022

{{< generation-table "2022" >}}

### 2021

{{< generation-table "2021" >}}

### 2020

{{< generation-table "2020" >}}

### 2019

{{< generation-table "2019" >}}

> Neoverse targets datacenter and infrastructure; Cortex-A/X target mobile and client.

### 2018

{{< generation-table "2018" >}}

 > AE variants add safety features (e.g. lockstep) commonly used in Automotive.

### 2017

{{< generation-table "2017" >}}

### 2016

{{< generation-table "2016" >}}

### 2015

{{< generation-table "2015" >}}

### 2014

{{< generation-table "2014" >}}

### 2012

{{< generation-table "2012" >}}

### 2010

{{< generation-table "2010" >}}

## ARM Mali GPUs

{{< category-list path="soc-manufacturers/arm/mali-gpu" >}}

## ARM Ethos NPUs

{{< category-list path="soc-manufacturers/arm/ethos-npu" >}}