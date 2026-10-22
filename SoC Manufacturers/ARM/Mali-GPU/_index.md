---
weight: 1
linktitle: Arm Mali GPU
title: ARM Mali GPU Architecture, Userspace Drivers (Mali UMD/DDK, Panfrost) and Kernel Drivers (Panfrost, Panthor)
summary: ARM Mali GPU architecture, userspace drivers (proprietary Mali UMD/DDK and open-source Panfrost), and kernel drivers (Panfrost and Panthor)
images:
- Arm-Mali-Transparent.png
icon: Arm-Mali-Transparent.png
categories:
- gpu
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

![Arm Mali GPU Logo](Arm-Mali-Transparent.png?h=100&f=webp)

# Mali-GPU

Mali is ARM's family of graphics processing units (GPUs) designed for mobile and embedded systems. Mali GPUs support various graphics APIs including OpenGL ES, OpenCL, and Vulkan on both the propietary and open source driver stacks. The open source drivers inside MESA add proper OpenGL support too. Starting with Valhall (v11) the brand Immortalis was introduced for the flagship tier.

## Mali GPU Userspace Driver

{{% columns %}}
- ### Proprietary Mali UMD<br>(User Mode Driver)
  ARM provides proprietary User Mode Driver (UMD). These drivers offer optimized performance and full feature support for ARM's proprietary Mali GPU implementations.
  
  **Features:**
  - Optimized performance
  - Proprietary support and updates
  - Used in production on many commercial devices

- ### Opensource Panfrost inside **MESA**
  The Panfrost driver stack includes an OpenGL ES & regular OpenGL implementation for Arm Mali GPUs for Midgard and newer microarchitectures.
  
  **Features:**
  - Community-driven development
  - GPL-licensed (free and open)
  - PanVK for Vulkan 1.4 support
  - Transparent code and security

  Official Website: [Panfrost Landing Page](https://docs.mesa3d.org/drivers/panfrost.html)

{{% /columns %}}

> The propietary driver stack is at version r54 since August 2025.

## Mali GPU Kernel Driver

{{% columns %}}
- ### Proprietary Mali DDK<br>(Device Driver Kit)
  ARM's proprietary kernel driver component provides direct hardware access and low-level GPU management for the Mali GPU. It works alongside the proprietary UMD.
  
  **Features:**
  - Direct hardware access
  - Optimized resource management
  - Integrated with proprietary UMD

  **Downsides**
  - Proprietary implementation
  - Starting from DDK version r52, GPUs up to Bifrost are no longer supported.

- ### Opensource Panfrost / Panthor / Tyr
  Panfrost and Panthor are open-source drivers for Mali GPUs developed by the community and collaborating organizations (Mainly collabora with the support of ARM). Panfrost supports older Mali GPU generations (Midgard and newer), while Panthor is the modern replacement supporting newer CSF architectures starting with v10 Valhall.

  Tyr is the upcoming Rust implementation of Panthor.
  
  **Features:**
  - Part of the mainline Linux kernel
  - Active community maintenance
  - Transparent hardware abstraction

{{% /columns %}}

---

## ARM Mali GPUs & Generations

### 2026

{{< generation-table "2026" >}}

 
> The Mali G2 Ultra NX (will exist as a 12 and 16 core variant) according to Genshin Impact's Vulkan whitelist
>
> The Mali TMAX / TMEX Immortalis also comes from the GI's Vulkan whitelist and there is no further information about it yet
>
> Names are confirmed by [Android 17 Kernel 6.18 Panthor Driver SDK](https://gitlab.arm.com/gpu/arm-mali-gpu-for-linux/-/blob/4b41d1102eaf1064ea0445215e4b52383add2342/drivers/gpu/drm/panthor/panthor_props.c#L255-266) and NX stands for Neural present and is a suffix like Immortalis

### 2025

{{< generation-table "2025" >}}

### 2024

{{< generation-table "2024" >}}

### 2023

{{< generation-table "2023" >}}

### 2022

{{< generation-table "2022" >}}

> **Note:** Immortalis (G715, G720, G925) share the same architecture version as their Mali siblings (v11, v12, v13); the Linux kernel distinguishes them by **10+ shader cores** and **hardware ray intersection** support, not by a different arch version. Utgard-based GPUs are supported by the Lima driver; Midgard and newer are supported by Panfrost/Panthor.
> <br>**Source**: [Linux Kernel - Panthor_hw.c](https://github.com/torvalds/linux/blob/master/drivers/gpu/drm/panthor/panthor_hw.c)

### 2021

{{< generation-table "2021" >}}

### 2020

{{< generation-table "2020" >}}

### 2019

{{< generation-table "2019" >}}

### 2018

{{< generation-table "2018" >}}

### 2017

{{< generation-table "2017" >}}

### 2016

{{< generation-table "2016" >}}

### 2015

{{< generation-table "2015" >}}

### 2013

{{< generation-table "2013" >}}

### 2012

{{< generation-table "2012" >}}

### 2011

{{< generation-table "2011" >}}

### 2010

{{< generation-table "2010" >}}

### 2008

{{< generation-table "2008" >}}

### 2007

{{< generation-table "2007" >}}

### 2005

{{< generation-table "2005" >}}
