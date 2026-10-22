---
weight: 3
title: Board Template
summary: Template for a single-board computer page with gallery, board-specs.yaml and OS list.
---

# Board Template

Create `SoC Manufacturers/<Vendor>/<SoC>/Boards/<Board-Name>/` with:

- `_index.md` – the page below
- `board-specs.yaml` – the board specifications, rendered by `{{</* board-specs */>}}`
- `images/` – pictures named `<board-name>-01.webp`, `<board-name>-02.webp`, …

In the front matter:

- `tags` holds the SoC part number, which lists the board on the SoC page.
- `boards` holds the board ID. Operating system pages list the same ID to show up under **Available OS images**.

## `_index.md`

```markdown
---
weight: 1
title: Vendor Board Name
categories:
- board
tags:
- SOC123
boards:
- Vendor-Board-Name
board-vendor:
- Vendor
summary: "Vendor Board Name single-board computer - SOC123 processor, key features in one sentence"
images:
- images/vendor-board-name-01.webp
---

# Vendor Board Name

## Board Pictures
{{</* gallery match="images/*" sortOrder="asc" rowHeight="150" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=true previewType="blur" embedPreview=true loadJQuery=true */>}}

## Hardware
{{%/* details title="Specs" open=true */%}}
{{</* board-specs */>}}
{{%/* /details */%}}

## Available OS images

{{</* list-board-available-os */>}}

## Documentation / Links

- [Vendor Docs](https://example.com)

## Benchmarks

## Guides

## Articles
```

## `board-specs.yaml`

`{{</* board-specs */>}}` renders two tables: the SoC table, taken from the `specs.yaml` of the SoC page above the board, and the board table from this file. Only describe what the board itself has. CPU, GPU, NPU and video specs come from the SoC.

Numbers are bare and in the unit the key names. Leave out anything you cannot source.

```yaml
memory:
  types: [{ type: "LPDDR4X", mts: 4266 }]
  bus_bits: 64
  sizes_gb: [4, 8, 16]
storage: ["eMMC module connector", "16 MB SPI flash (bootloader)", "microSD (SDR104)"]
pcie:
  - { count: 1, slot: "M.2 M-Key", gen: 3, lanes: 4, note: "2280 NVMe SSD" }
  - { count: 1, slot: "M.2 E-Key", gen: 2, lanes: 1 }
usb:
  - { count: 1, version: "3.1 Gen1", connector: "Type-C", note: "Power Delivery" }
  - { count: 2, version: "3.1 Gen1", connector: "Type-A" }
  - { count: 2, version: "2.0", connector: "Type-A" }
ethernet:
  - { count: 1, gbps: 2.5, note: "RTL8125, PoE with add-on HAT" }
wifi: "Wi-Fi 6 (onboard)"
bluetooth: "5.2"
display:
  outputs: ["1× HDMI 2.1 (8K@60)", "1× MIPI DSI"]
  inputs: ["1× HDMI 2.0 (4K@60)"]
camera: "2× 4-lane MIPI CSI"
gpio: "40-pin header"
power: "USB Type-C PD, 5 V–20 V"
rtc: "Battery connector"
dimensions_mm: { w: 100, h: 72 }
```

Other optional fields:

| Field | Example |
|-------|---------|
| `name` | `"Radxa Rock 5B"` – table header, defaults to the page title |
| `revision` | `"1.1"` |
| `soc.page` | `"/docs/soc-manufacturers/rockchip/rk3588"` – only if the board does not sit under its SoC page |
| `soc.part` | `"QCS8275"` – which part of a multi-part `specs.yaml` |
| `soc.name` | `"Rockchip RK3588S"` – SoC table header, e.g. for a variant |
| `soc.notes` | `["CPU clocked at up to 1.6 GHz on this board"]` |
| `can` | `{ count: 2, fd: true }` |
| `mcu` | `{ name: "STM32U585", core: "Cortex-M33", max_mhz: 160 }` – adds a microcontroller table |
| `weight_g` | `46` |
| `audio`, `cooling`, `sensors`, `debugging`, `enclosure`, `form_factor`, `temperature` | text or list |
| `other` | `[{ name: "Throughput", value: "Up to 26 Gbps" }]` – rows the schema lacks |

The full list is at the top of `layouts/shortcodes/board-specs.html` in the SBCwiki repository.

## Benchmark scores

Benchmark results are stored in `data/scores/<board-id>.yaml` in the SBCwiki repository and feed the [Rankings]({{< relref "/docs/rankings" >}}). Open an issue or pull request with your results and the exact OS, kernel and driver versions used.
