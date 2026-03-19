---
weight: 2
linktitle: Arm Mali GPU
title: ARM Mali GPU Architecture, Userspace Drivers (Mali UMD/DDK, Panfrost) and Kernel Drivers (Panfrost, Panthor)
summary: ARM Mali GPU architecture, userspace drivers (proprietary Mali UMD/DDK and open-source Panfrost), and kernel drivers (Panfrost and Panthor)
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

> The propietary driver stack is at version r54 sice August 2025.

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

### Upcoming

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| "6th Gen" Magni (v15) | Mali G2-Ultra | Flagship |
| "6th Gen" Magni (v15) | Mali G2-Premium | Mid-Range |
| "6th Gen" Magni (v15) | Mali G2-Pro | Entry |

> Names are a guess for the upcoming Magni v15 Generation

### 2025

| Micro Architecture | Name | Class |
|-------------------|------|-------|
| "5th Gen" (v14) | Mali G1-Ultra | Flagship |
| "5th Gen" (v14) | Mali G1-Premium | Mid-Range |
| "5th Gen" (v14) | Mali G1-Pro | Entry |

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
