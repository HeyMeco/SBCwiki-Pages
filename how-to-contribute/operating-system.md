---
weight: 4
title: Operating System Template
summary: Template for an operating system page that links to supported boards.
---

# Operating System Template

Create `Operating Systems/Linux/<Distribution>/_index.md` and put the logo next to it.

List every supported board under `boards` using the exact ID from the board page. The board then shows this OS under **Available OS images**, and this page lists the board.

```markdown
---
weight: 10
title: Distribution Name
icon: Distribution-Logo.png
summary: One sentence describing the distribution and who it is for.
categories:
- os
boards:
- Vendor-Board-Name
- Other-Board-Name
---
![Distribution Name Logo](Distribution-Logo.png?h=150)

# Distribution Name

[Official Website](https://example.com)

## Description

## Supported Boards

{{</* list-os-boards */>}}

## Installation
```
