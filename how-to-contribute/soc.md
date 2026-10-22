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

More fields (ISP, cache, SATA, CAN, TDP, …) are documented at the top of `layouts/shortcodes/soc-specs.html` in the SBCwiki repository. Look at an existing SoC such as RK3576 for a complete example.

- **CPU, GPU and NPU names** link to their generation automatically. Write the name as the vendor does (`Cortex-A76`, `Mali-G610 MP4`, `Adreno 643`). If it is not found, add it to `ARM/cpus.yaml` or the GPU family's `gpus.yaml` rather than setting `link`.
- **Mesa support** is looked up from the GPU family's `mesa.yaml`. `vendor_apis` holds only what the vendor's own driver supports.
- **Several parts in one file:** when one page covers several chips (e.g. a lineup page), list each as its own entry under `parts`. The page then shows a comparison table, and boards pick theirs with `soc.part` in `board-specs.yaml`.

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
