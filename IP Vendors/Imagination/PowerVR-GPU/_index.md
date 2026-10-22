---
weight: 1
linktitle: PowerVR GPU
title: "Imagination PowerVR GPU Architecture, Userspace Drivers (IMG DDK, Mesa PowerVR Vulkan) and Kernel Drivers (pvrsrvkm, powervr)"
description: "Imagination PowerVR GPUs (Rogue Series 6/7/8, A-Series, B-Series): Mesa PowerVR Vulkan driver support per BVNC, the proprietary IMG DDK, and the mainline Linux powervr kernel driver."
summary: "Imagination PowerVR GPUs (Rogue Series 6/7/8, A-Series, B-Series): Mesa PowerVR Vulkan driver support per BVNC, the proprietary IMG DDK, and the mainline Linux powervr kernel driver."
categories:
- gpu
ip-vendors:
- Imagination
keywords: ["Imagination", "PowerVR", "PowerVR GPU", "Rogue", "BXM-4-64", "BXS-4-64", "AXE-1-16M", "BVNC", "Mesa", "Vulkan", "powervr", "pvrsrvkm", "IMG DDK", "Linux GPU driver"]
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
</style>

# PowerVR-GPU

PowerVR is Imagination Technologies' family of tile-based deferred rendering (TBDR) GPUs, licensed as IP to SoC vendors. All parts from Series6 onwards share the **Rogue** architecture lineage, continued by the A-, B-, C-, D- and E-Series. Every PowerVR core is identified by its **BVNC** (Branch.Version.Number.Config): one product name can cover several BVNCs with different features and errata, so driver support is tracked per BVNC, not per product name.

## PowerVR GPU Userspace Driver

{{% columns %}}
- ### Proprietary IMG DDK<br>(Driver Development Kit)
  Imagination provides a proprietary userspace driver stack to its licensees, shipped in vendor BSPs.

  **Features:**
  - OpenGL ES 3.2, Vulkan 1.3 and OpenCL 3.0 on current B-Series parts
  - Used in production on commercial devices

- ### Opensource PowerVR Vulkan inside **MESA**
  The Mesa PowerVR driver is a Vulkan-only driver, developed by Imagination in upstream Mesa. There is no PowerVR OpenGL driver in Mesa.

  **Features:**
  - MIT-licensed (free and open)
  - Vulkan 1.2, conformant on BXM-4-64 (`36.52.104.182`) and BXS-4-64
  - GPUs before Series6 lack the hardware features Vulkan needs and will not be supported

  Official Website: [Mesa PowerVR Driver](https://docs.mesa3d.org/drivers/powervr.html)

{{% /columns %}}

> On GPUs that are not yet conformant to any Vulkan version, Mesa refuses to run unless `PVR_I_WANT_A_BROKEN_VULKAN_DRIVER=1` is set in the environment.

## PowerVR GPU Kernel Driver

{{% columns %}}
- ### Proprietary pvrsrvkm
  The kernel side of the IMG DDK, an out-of-tree module shipped in vendor BSP kernels and used together with the proprietary userspace driver.

  **Downsides:**
  - Out-of-tree, tied to specific vendor kernel branches

- ### Opensource powervr
  `powervr` (`drivers/gpu/drm/imagination`) is the mainline Linux DRM driver for PowerVR Rogue-based GPUs, merged in Linux 6.8 and used by the Mesa PowerVR Vulkan driver. It needs GPU firmware from linux-firmware.

  **Features:**
  - Part of the mainline Linux kernel
  - Developed and maintained by Imagination
  - RISC-V SoC support since Linux 6.18

{{% /columns %}}

---

## PowerVR GPUs in Mesa

GPUs as listed in the [Mesa PowerVR driver documentation](https://docs.mesa3d.org/drivers/powervr.html), grouped by support status.

### Actively developed

{{< generation-table "actively-developed" >}}

### Partially supported

Core-specific features and workarounds are likely missing: simple Vulkan applications may run, but expect instability and corruption.

{{< generation-table "partially-supported" >}}

### Unsupported

Device info and firmware exist in Mesa for these GPUs, usually out of community interest, but no support is guaranteed and they are not under active development.

{{< generation-table "unsupported" >}}
