---
weight: 1
title: SoC Vendor Template
summary: Template for an SoC manufacturer page that lists its SoCs and tutorials.
---

# SoC Vendor Template

Create `SoC Manufacturers/<Vendor>/_index.md`. Put the vendor logo in the main repository under `static/assets/<vendor>/` and reference it as shown.

Pick a short tag prefix for the vendor (Rockchip uses `RK`) and use it on every SoC page: `SOC-<PREFIX>` for current chips, `SOC-<PREFIX>-Upcoming` for announced ones and `TuT-<PREFIX>` for tutorials.

```markdown
---
weight: 10
title: Vendor Name
icon: /assets/vendor-name/Vendor-Logo.png
categories:
- soc-vendors
soc-vendors:
- Vendor Name
bookCollapseSection: true
summary: All Vendor Name SoCs, boards, and development resources on sbcwiki.com
---

![Vendor Name Logo](assets/vendor-name/Vendor-Logo.png?h=100)

## Current Vendor Name SoCs

{{</* taglist SOC-PREFIX */>}}

## Upcoming Vendor Name SoCs

{{</* taglist SOC-PREFIX-Upcoming */>}}

## Tutorials

{{</* taglist TuT-PREFIX */>}}

---

{{%/* details "Archive" "..." */%}}

## Archived SoCs

- Vendor Name OLD123

{{%/* /details */%}}
```
