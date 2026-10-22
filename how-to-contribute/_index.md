---
weight: 3
bookFlatSection: true
bookCollapseSection: true
title: "How to Contribute"
description: How to add or improve pages on SBCwiki - SoC vendors, SoCs, boards and operating systems - with copy-paste Markdown templates.
summary: Add or improve SBCwiki pages with Markdown templates.
---

# How to Contribute

The SBCwiki documentation is open to everyone. Every page is a Markdown file in the [SBCwiki-Pages](https://github.com/HeyMeco/SBCwiki-Pages) repository, so fixing a typo, adding a board or documenting a new SoC is a pull request away. News articles are written by SBCwiki authors only.

## Workflow

1. **Small fixes:** open the page on GitHub, click the pencil icon, edit, and submit the pull request GitHub proposes.
2. **New pages:** fork [SBCwiki-Pages](https://github.com/HeyMeco/SBCwiki-Pages), create a branch, add your files and open a pull request against `main`.
3. Describe what you changed and link your sources (vendor datasheets, TRMs, official docs). Specs without a source may be held back until they can be verified.

## Where pages live

Each page is a folder with an `_index.md` (a page bundle). Images and data files sit next to it.

```text
SoC Manufacturers/
├── links.json                   ← extra link targets for spec tables
├── ARM/
│   ├── cpus.yaml                ← Arm CPU core generations
│   └── Mali-GPU/
│       ├── gpus.yaml            ← Mali GPU generations
│       └── mesa.yaml            ← Mesa driver support per GPU architecture
├── Rockchip/                    ← SoC vendor page
│   ├── _index.md
│   └── RK3588/                  ← SoC page
│       ├── _index.md
│       ├── specs.yaml           ← SoC specifications
│       ├── Boards/
│       │   ├── _index.md        ← hidden list page, copy from a sibling SoC
│       │   └── Radxa-Rock-5B/   ← board page
│       │       ├── _index.md
│       │       ├── board-specs.yaml  ← board specifications
│       │       └── images/
│       │           └── radxa-rock-5b-01.webp
│       └── Variants/
│           └── RK3588s/         ← cut-down variant, with its own Boards/ folder
Operating Systems/
└── Linux/
    └── Armbian/                 ← operating system page
        ├── _index.md
        └── Armbian-Logo.png
```

Folder names become the URL: `SoC Manufacturers/Rockchip/RK3576` is served at `/docs/soc-manufacturers/rockchip/rk3576/`. Use the part number or product name with dashes instead of spaces, e.g. `Radxa-Rock-4D`.

## How pages are linked together

Pages find each other through front matter values, not hand-written lists. Keep these consistent:

| Field | Used on | Purpose |
|-------|---------|---------|
| `tags: [SOC-RK]` | SoC page | Lists the SoC on its vendor page (`{{</* taglist SOC-RK */>}}`). Use `SOC-RK-Upcoming` style tags for unreleased chips. |
| `tags: [RK3576]` | Board page | Lists the board as a card on its SoC page (`{{</* taglist tag="RK3576" style="cards" */>}}`). |
| `boards: [Radxa-Rock-4D]` | Board and OS pages | Connects boards and operating systems. The value must match exactly on both pages. |
| `categories: [os]` | OS page | Marks the page as an operating system. |
| `summary` | All pages | Shown in cards, search results and link previews. Keep it to one sentence. |

## Specification data

Spec tables are not written in Markdown. They are generated from YAML files next to the page, so the same numbers feed the SoC page, every board page and the site-wide comparisons.

| File | Rendered by | Contains |
|------|-------------|----------|
| `specs.yaml` | `{{</* soc-specs */>}}` on the SoC page | The SoC: CPU clusters, memory, GPU, NPU, VPU, I/O. See the [SoC template]({{< relref "soc" >}}). |
| `board-specs.yaml` | `{{</* board-specs */>}}` on the board page | Only what the board adds: RAM sizes, connectors, ports, power. The SoC table is pulled in automatically. See the [board template]({{< relref "board" >}}). |
| `ARM/cpus.yaml`, `ARM/Mali-GPU/gpus.yaml`, `Qualcomm/Adreno-GPU/gpus.yaml` | `{{</* generation-table */>}}` on those pages | CPU core and GPU generations. SoC tables link core and GPU names here automatically. |
| `ARM/Mali-GPU/mesa.yaml`, `Qualcomm/Adreno-GPU/mesa.yaml` | SoC spec tables | Open-source (Mesa) driver support. Edit it here, never in a `specs.yaml`. |
| `SoC Manufacturers/links.json` | SoC spec tables | Link targets for NPUs and names the generation files lack. |

Rules for all spec files:

- Numbers are bare and in the unit the key names: `max_ghz: 2.4`, never `"2.4 GHz"`.
- Every field is optional except `name` in `specs.yaml`. Leave out what you cannot source.
- Text values are inline Markdown, so links, **bold** and `<br>` work.
- If an SoC uses a CPU core or GPU that is not in the generation files yet, add it there instead of hard-coding a link.
- The full field lists are documented at the top of `layouts/shortcodes/soc-specs.html` and `layouts/shortcodes/board-specs.html` in the SBCwiki repository.

## Writing guidelines

- Write facts, not marketing. "4× Cortex-A76 up to 2.4 GHz" beats "blazing fast".
- Link the source for every specification you add.
- Images: use WebP or AVIF, crop to the board, no watermarks, and only upload pictures you own or are allowed to share.
- One board or SoC per pull request makes review faster.

## Previewing locally (optional)

The site is built with [Hugo](https://gohugo.io/) (extended). Clone the main [SBCwiki](https://github.com/HeyMeco/SBCwiki) repository with submodules, then run the dev server:

```bash
git clone --recurse-submodules https://github.com/HeyMeco/SBCwiki.git
cd SBCwiki
hugo server
```

Your page appears at `http://localhost:1313/docs/...`. Make your edits inside `content/docs`, which is the SBCwiki-Pages repository.

## Templates

Copy a template into a new folder as `_index.md` and fill in the placeholders.

{{< category-list >}}
