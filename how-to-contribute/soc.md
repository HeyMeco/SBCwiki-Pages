---
weight: 2
title: SoC Template
summary: Template for an SoC page with a specs.yaml specification table and board list.
---

# SoC Template

Create `SoC Manufacturers/<Vendor>/<SoC>/` with three files:

- `_index.md` – the page below
- `specs.yaml` – the specifications, rendered by `{{</* soc-specs */>}}`
- `Boards/_index.md` – a hidden list page, copy it from any other SoC

## `_index.md`

```markdown
---
weight: 10
title: Vendor Name SOC123
soc-series:
- SERIES
soc:
- SOC123
tags:
- SOC-PREFIX
summary: Vendor Name SOC123 - core configuration, GPU, NPU TOPS and video capabilities in one sentence.
---
# Vendor Name SOC123

## General Specifications
{{%/* details title="Specs" open=true */%}}

{{</* soc-specs */>}}

{{%/* /details */%}}

---

## Linux Support
{{%/* columns */%}}
- ### Vendor BSP
  - Current version based on: 6.1

- ### Mainline kernel
  - [ ] Fully supported
  - [x] Works but not all features are implemented.

{{%/* /columns */%}}

---

## Documentation
- [Datasheet](https://example.com)
- [Technical Reference Manual](https://example.com)

---

## Boards with SOC123

{{</* taglist tag="SOC123" style="cards" */>}}
```

## `specs.yaml`

Numbers are bare and in the unit the key names (`max_ghz: 2.2`, never `"2.2GHz"`). Every field except `name` is optional, so leave out what you cannot source.

```yaml
parts:
  - name: "Vendor Name SOC123"
    process_nm: 8
    cpu:
      clusters:                       # fastest cluster first
        - { cores: 4, core: "Cortex-A76", max_ghz: 2.4 }
        - { cores: 4, core: "Cortex-A55", max_ghz: 1.8 }
    memory:
      types: ["LPDDR4X", "LPDDR5"]
      bus_bits: 64
      max_gb: 32
    gpu:
      name: "Mali-G610 MP4"
      vendor_apis: { opengl_es: "3.2", vulkan: "1.3", opencl: "2.2" }
    npu:
      tops: 6
      datatypes: ["INT4", "INT8", "INT16", "FP16"]
    vpu:
      decode:
        - { res: "8K", fps: 60, codecs: ["H.265", "VP9", "AV1"] }
      encode:
        - { res: "8K", fps: 30, codecs: ["H.264", "H.265"] }
    display: { max: "8K@60", outputs: ["HDMI 2.1", "eDP 1.4", "MIPI DSI"] }
    pcie: [{ count: 1, gen: 3, lanes: 4 }]
    usb: [{ count: 2, version: "3.2 Gen1" }, { count: 2, version: "2.0" }]
    ethernet: [{ count: 2, gbps: 1 }]
```

More fields (ISP, cache, SATA, CAN, TDP, …) are listed in the [field reference](#field-reference) below. Look at an existing SoC such as RK3576 for a complete example.

- **CPU, GPU and NPU names** link to their generation automatically. Write the name as the vendor does (`Cortex-A76`, `Mali-G610 MP4`, `Adreno 643`). If it is not found, add it to `ARM/cpus.yaml` or the GPU family's `gpus.yaml` rather than setting `link`.
- **Mesa support** is looked up from the GPU family's `mesa.yaml`. `vendor_apis` holds only what the vendor's own driver supports.
- **Several parts in one file:** when one page covers several chips (e.g. a lineup page), list each as its own entry under `parts`. The page then shows a comparison table, and boards pick theirs with `soc.part` in `board-specs.yaml`.

## Field reference

Every field `specs.yaml` understands. All are optional except `name`; `notes` may be a string or a list wherever it appears. Text values are inline Markdown.

```yaml
label: "SoC"                      # left header cell (default "SoC", or "Part" for several)
parts:
  - name: "Rockchip RK3588"
    link: "/docs/..."             # name links here in comparison tables
    codename: "Lemans"
    process_nm: 8
    process_note: "LPC FinFET"    # shown as "8 nm (LPC FinFET)"
    cpu:
      clusters:                   # one entry per core type, fastest first
        - { cores: 4, core: "Cortex-A76", max_ghz: 2.4 }
        - { cores: 4, core: "Cortex-A55", max_ghz: 1.8, note: "LITTLE" }
        # also: base_ghz (all-core clock; max_ghz is then the boost clock),
        #       max_mhz (instead of max_ghz for slow cores), link (overrides the automatic link)
      cores: 6                    # only when the split into clusters is not known
      core: "Cortex-A78 and Cortex-A55"   # likewise
      max_ghz: 2.1                # chip-wide peak when clusters carry no clocks
      isa: "Armv9.2"
      cache: [{ level: "L3", mb: 4 }, { level: "L2", mb: 2, per: "core" }]
      notes: "free text"
    mcu: [{ cores: 1, core: "Cortex-M7", max_mhz: 800 }]   # not counted as CPU cores
    memory:
      types: ["LPDDR4X", { type: "LPDDR5", mts: 6400 }]   # mts = data rate in MT/s
      bus_bits: 64
      channels: 12
      max_gb: 16
      bandwidth_gbs: 68           # GB/s
      ecc: true                   # or "inline"
    gpu:
      name: "Mali-G610 MP4"
      link: "/docs/..."
      max_mhz: 1000
      gflops: 64                  # or tflops: 4.6 (FP32)
      vendor_apis: { opengl_es: "3.2", vulkan: "1.2", opencl: "2.2", openvg: "1.1", directx: "12" }
      # Mesa support comes from the GPU family's mesa.yaml. Only if needed:
      # mesa: false               # hide the Mesa line for this GPU
      # mesa: { apis: { vulkan: "1.3" }, drivers: { vulkan: "PanVK" }, note: "…" }   # replace it
    npu:
      name: "Hexagon"
      tops_dense: 350             # vendor says dense
      tops_sparse: 700            # vendor says sparse
      tops: 6                     # vendor does not say which
      tops_precision: "INT8"
      # For a range ("20–40 TOPS") store the highest value and say so in notes.
      datatypes: ["INT4", "INT8", "INT16", "FP16"]
    vpu:
      name: "Arm-China Linlon V8"
      decode: [{ res: "8K", fps: 60, codecs: ["H.265", "VP9"] }]   # res: 16K/8K/4K/1440p/1080p/720p
      encode: [{ res: "4K", fps: 30, codecs: ["H.264"] }]
    isp: { count: 2, max_mp: 48, mpixel_s: 500 }
    camera: ["2× MIPI CSI-2 (4-lane)"]
    display: { max: "4K@60 + 2K@60", outputs: ["HDMI 2.1", "eDP 1.4", "MIPI DSI"] }
    storage: ["eMMC 5.1", "UFS 2.1", "SD 3.0"]
    pcie: [{ count: 2, gen: 3, lanes: 1, note: "RC/EP" }]
    sata: { count: 1, gen: "3.0" }
    usb: [{ count: 1, version: "3.2 Gen1" }, { count: 2, version: "2.0" }]
    ethernet: [{ count: 2, gbps: 2.5, note: "TSN" }]   # gbps 0.1 renders as 100 Mbit
    wifi: "Wi-Fi 7"
    bluetooth: "5.4"
    can: { count: 5, fd: true }
    io: "…"                       # io, audio, dsp, security: text or list
    tdp_w: { min: 230, max: 420 } # or a single number
    package: "…"                  # package, temperature, os, availability: text or list
    other: [{ name: "Target", value: "Edge AI" }]       # rows the schema lacks
```

If you need a field that is not listed here, use `other` and open an issue on [SBCwiki-Pages](https://github.com/HeyMeco/SBCwiki-Pages/issues) to suggest it.

## Variants

A cut-down or binned version of an SoC goes in `<SoC>/Variants/<Variant>/` with its own `_index.md` and `Boards/` folder. If the variant has no `specs.yaml` of its own, its boards use the parent SoC's table and set `soc.name` (e.g. `"Rockchip RK3588S"`) and `soc.notes` in `board-specs.yaml` to describe the difference.

## `Boards/_index.md`

```markdown
---
weight: 10
title: Boards
bookCollapseSection: true
bookHidden: true
noindex: true
---
```
