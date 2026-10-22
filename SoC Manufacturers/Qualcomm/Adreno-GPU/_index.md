---
weight: 1
linktitle: Adreno GPU
title: "Qualcomm Adreno GPU Architecture, Specs & Drivers (Adreno UMD, Mesa Freedreno / Turnip, KGSL, drm/msm)"
description: "Complete guide to Qualcomm Adreno GPUs (600, 700, 800, X1 & X2 series): specifications, Vulkan support timeline, proprietary Adreno UMD/KGSL, and open-source Mesa Freedreno, Turnip, and Linux drm/msm drivers."
summary: "Complete guide to Qualcomm Adreno GPUs (600, 700, 800, X1 & X2 series): specifications, Vulkan support timeline, proprietary Adreno UMD/KGSL, and open-source Mesa Freedreno, Turnip, and Linux drm/msm drivers."
images:
- Qualcomm_official_adreno_logo.jpeg
icon: Qualcomm_official_adreno_logo.jpeg
categories:
- gpu
soc-vendors:
- Qualcomm
keywords: ["Qualcomm", "Adreno", "Adreno GPU", "Freedreno", "Turnip", "Mesa", "Vulkan", "KGSL", "drm/msm", "Adreno UMD", "Adreno 600", "Adreno 700", "Adreno 800", "Adreno X1", "Adreno X2", "Snapdragon", "Dragonwing", "GPU specifications", "Linux GPU driver"]
---

<style>
/* On this page only: hide H3+ in all TOC variants */
.book-toc nav ul ul,      /* desktop sidebar */
.book-header nav ul ul {  /* inline header TOC */
  display: none;
}

/* On this page only: column widths for 3-column tables */
.markdown table {
  width: 100%;
  table-layout: fixed;
}
.markdown table th:nth-child(1),
.markdown table td:nth-child(1) {
  width: 25%;
}
.markdown table th:nth-child(2),
.markdown table td:nth-child(2) {
  width: 20%;
}
.markdown table th:nth-child(3),
.markdown table td:nth-child(3) {
  width: 55%;
}
</style>

![Qualcomm Adreno GPU Logo](Qualcomm_official_adreno_logo.jpeg?h=100&f=webp)

# Adreno-GPU

Adreno (an anagram of *Radeon*, originating from AMD's Imageon handheld graphics division acquired by Qualcomm in 2009) is Qualcomm's family of integrated graphics processing units (GPUs) used across Snapdragon and Dragonwing SoCs. Adreno GPUs feature a unified shader model with a tile-based flex rendering architecture (`FlexRender`) that dynamically switches between immediate-mode and tile-based rendering, paired with Universal Bandwidth Compression (`UBWC`) and dedicated on-chip Graphics Memory (`GMEM`).

Adreno GPUs support OpenGL ES, OpenCL, Vulkan, and DirectX 11/12 on the proprietary driver stack, while the open-source Freedreno stack inside Mesa adds full desktop OpenGL 4.6 and Vulkan 1.3/1.4 support.

## Adreno GPU Userspace Driver

{{% columns %}}
- ### Proprietary Adreno UMD<br>(User Mode Driver)
  Qualcomm provides proprietary User Mode Drivers (UMD) for Android, Windows on ARM (including the *Adreno Control Panel*), and downstream Linux/Embedded platforms.

  **Features:**
  - Optimized day-one hardware support and power efficiency
  - Snapdragon Elite Gaming features (Adreno Frame Motion Engine, VRS Pro, Game Super Resolution)
  - DirectX 11 / 12, OpenGL ES 3.2, Vulkan 1.3 / 1.4, and OpenCL 2.0 / 3.0 FP support
  - Used in production on commercial Android smartphones, XR headsets, and Windows on ARM PCs

- ### Opensource Freedreno inside **MESA**
  The Freedreno project inside Mesa 3D provides open-source userspace drivers for Qualcomm Adreno GPUs (`a2xx` through `a8xx`).

  **Features:**
  - **Freedreno** Gallium3D driver for full desktop OpenGL 4.6 & OpenGL ES 3.2
  - **Turnip** Vulkan 1.3 / 1.4 driver for `a6xx`, `a7xx`, and `a8xx` generations
  - **Rusticl** / Clover OpenCL support
  - Supports both mainline Linux (`drm/msm`) and stock Android vendor kernels (`kgsl` backend)
  - MIT-licensed (free and open)

  Official Website: [Freedreno Landing Page](https://docs.mesa3d.org/drivers/freedreno.html)

{{% /columns %}}

> Turnip (`vulkan.freedreno`) is widely used both on mainline Linux SBCs/laptops and inside Android containers/emulators (via the `kgsl` backend) for DirectX-to-Vulkan translation layers like DXVK and VKD3D-Proton.
>
> **Note:** Newer DXVK versions require the `storageBuffer8BitAccess` Vulkan feature, which on Turnip is only exposed on `a7xx`-class Adreno GPUs — `a6xx`-class parts (Adreno 600 series) lack it. For games on `a6xx`-class hardware, use **Proton 11** (or another build bundling an older DXVK that predates the `storageBuffer8BitAccess` requirement) to avoid the gap.

### Vulkan Support Timeline

{{% steps %}}
1. ## Adreno 400 & 500 Series (`a4xx` / `a5xx`) — Vulkan 1.0 / 1.1
   - **Proprietary UMD:** Introduced **Vulkan 1.0** on Adreno 400/500 series, with **Vulkan 1.1** added via driver updates on Adreno 500 series.
   - **Mesa Turnip:** Not supported (Turnip targets `a6xx` and newer; `a4xx` and `a5xx` are supported by the Freedreno Gallium3D OpenGL/ES driver).

2. ## Adreno 600 Series (`a6xx_gen1`–`a6xx_gen4`) — Vulkan 1.1 to 1.3
   - **Proprietary UMD:** Launched with **Vulkan 1.1**, with later `a6xx_gen3` / `a6xx_gen4` platforms and Windows/Android driver updates reaching **Vulkan 1.2 / 1.3** (Note: cut-down `a6xx_gen1_low` parts like Adreno 702 lack full Vulkan compute/geometry pipelines).
   - **Mesa Turnip:** Official Khronos **Vulkan 1.3** conformance across `a6xx` (`a6xx_gen1` through `a6xx_gen4`), and **Vulkan 1.4** in recent Mesa releases.

3. ## Adreno 700 & X1 Series (`a7xx_gen1`–`a7xx_gen3`) — Vulkan 1.3 / 1.4 & Ray Tracing
   - **Proprietary UMD:** Native **Vulkan 1.3** (and **Vulkan 1.4** via driver updates), introducing hardware-accelerated **Vulkan Ray Tracing** (`VK_KHR_ray_query` / `VK_KHR_acceleration_structure` / `VK_KHR_ray_tracing_pipeline`) starting with `a7xx_gen2` (Adreno 740) and `a7xx_gen3` (Adreno 735 / 750).
   - **Mesa Turnip:** Official Khronos **Vulkan 1.4** conformance on `a7xx` (including Adreno X1-85 / X1-45 from Mesa 24.2+), with hardware ray intersection (`has_ray_intersection`) enabled on Adreno 735, 740, and 750.

4. ## Adreno 800 & X2 Series (`a8xx`) — Vulkan 1.4
   - **Proprietary UMD:** Ships with native **Vulkan 1.4** and full hardware ray tracing support on the sliced `a8xx` architecture.
   - **Mesa Turnip:** Initial `a8xx` bring-up in upstream Mesa targeting **Vulkan 1.4**.
{{% /steps %}}

## Adreno GPU Kernel Driver

{{% columns %}}
- ### Proprietary KGSL<br>(Kernel Graphics Support Layer)
  Qualcomm's downstream kernel driver (`msm_kgsl` / `/dev/kgsl-3d0`) provides low-level hardware access, memory management, and Graphics Management Unit (GMU) firmware control on Android and downstream Linux BSPs.

  **Features:**
  - Direct hardware access and GMU power/frequency management
  - Integrated with Qualcomm downstream BSPs and stock Android kernels
  - Supported by Mesa Freedreno/Turnip via the `kgsl` backend without replacing the vendor kernel

  **Downsides:**
  - Out-of-tree downstream driver (not merged into mainline Linux)
  - Tied to specific vendor kernel branches

- ### Opensource drm/msm
  `drm/msm` is the mainline Linux kernel Direct Rendering Manager (DRM/KMS) driver for Qualcomm Adreno GPUs and display processors (MDP4/MDP5/DPU).

  **Features:**
  - Part of the mainline Linux kernel (`drivers/gpu/drm/msm`)
  - Active community and Qualcomm upstream maintenance
  - Handles GPU command submission, GMU power management, per-process page tables, and display output

{{% /columns %}}

---

## Qualcomm Adreno GPUs & Generations (600 Series and Upwards)

### Adreno X Series (PC / Compute)

Designed for Qualcomm's Oryon-based Snapdragon X PC and industrial compute platforms, featuring wide 128-bit to 192-bit LPDDR5X memory interfaces and full DirectX 12.1 / Vulkan 1.3+ support.

{{< generation-table "adreno-x-series-pc--compute" >}}

> **Note:** In [`freedreno_devices.py`](https://gitlab.freedesktop.org/mesa/mesa/-/blob/main/src/freedreno/common/freedreno_devices.py), **Adreno X1-85** is defined under `CHIP.A7XX` / `a7xx_gen2` (internally `Adreno 741`) and **Adreno X1-45** is defined under `CHIP.A7XX` / `a7xx_gen2` (internally `Adreno 726`, derived from Adreno 725). Both are supported by Mesa Freedreno/Turnip starting from Mesa 24.2.

### Adreno 800 Series (2024–2026)

Introduced in late 2024, the Adreno 800 (`a8xx`) generation transitions to a **sliced architecture** where shaders and dedicated L2/GMEM cache blocks are partitioned into independent slices, alongside **UBWC v6** and Vulkan 1.3/1.4 support.

{{< generation-table "adreno-800-series-20242026" >}}

### Adreno 700 Series (2021–2024)

Introduced with the Snapdragon 8 Gen 1, the Adreno 700 (`a7xx`) family doubled FP32 ALU density per shader block and introduced hardware-accelerated **Ray Tracing** starting with the Adreno 740.

{{< generation-table "adreno-700-series-20212024" >}}

> **Note:** Based on Mesa's [`freedreno_devices.py`](https://gitlab.freedesktop.org/mesa/mesa/-/blob/main/src/freedreno/common/freedreno_devices.py):
> - **Adreno 702** is marketed in the 700 series, but in `freedreno_devices.py` it is defined under `CHIP.A6XX` with `[a6xx_base, a6xx_gen1_low]` (alongside Adreno 610/612) rather than `CHIP.A7XX`, with a halved register file (`reg_size_vec4 = 48`) and stripped-down hardware blocks (`# A702 cuts A LOT of things..`).
> - Within `CHIP.A7XX`, Mesa subdivides the family into `a7xx_gen1` (Adreno 710, 720, 730), `a7xx_gen2` (Adreno 725, 732, 740, and X1-85), and `a7xx_gen3` (Adreno 735, 750). Hardware ray intersection (`has_ray_intersection = True`) is only present on Adreno 735, 740, and 750.

### Adreno 600 Series (2018–2023)

Introduced in 2018 with the Snapdragon 845, the Adreno 600 (`a6xx`) architecture unified shader and compute pipelines with Direct3D 12_1, OpenGL ES 3.2, OpenCL 2.0/3.0, and Vulkan 1.1–1.3 support. It enjoys the most mature open-source support in Mesa's Freedreno and Turnip drivers.

{{< generation-table "adreno-600-series-20182023" >}}

> **Note:** Model numbers in the Adreno 600 series do not strictly reflect sub-architecture generation. In Mesa's [`freedreno_devices.py`](https://gitlab.freedesktop.org/mesa/mesa/-/blob/main/src/freedreno/common/freedreno_devices.py), `CHIP.A6XX` is divided into five sub-generations:
> - `a6xx_gen1_low` (`reg_size_vec4 = 48`): Adreno 610, 612, and 702
> - `a6xx_gen1` (`reg_size_vec4 = 96`): Adreno 615, 616, 618, 619, 620, and 630
> - `a6xx_gen2` (`reg_size_vec4 = 96`): Adreno 640 and 680
> - `a6xx_gen3` (`reg_size_vec4 = 64`): Adreno 613 and 650 (note that Adreno 613 is `gen3` while 615–620 are `gen1`)
> - `a6xx_gen4` (`reg_size_vec4 = 64`, `instr_cache_size = 127`): Adreno 642L, 643, 644, 660, 663, and 690 (making Adreno 642L/643/644 architecturally newer `gen4` parts than the `gen2` Adreno 640 and `gen3` Adreno 650)
>
> **Sources:** [Mesa — freedreno_devices.py](https://gitlab.freedesktop.org/mesa/mesa/-/blob/main/src/freedreno/common/freedreno_devices.py), [Wikipedia — Adreno](https://en.wikipedia.org/wiki/Adreno), and [Mesa 3D — Freedreno Driver Documentation](https://docs.mesa3d.org/drivers/freedreno.html)
