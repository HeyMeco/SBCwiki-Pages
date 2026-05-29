---
weight: 0
title: ARM Silicon
linktitle: ARM Silicon
summary: Explore the ARM AGI CPU family, Arm's first production silicon for AI infrastructure. View specs and datasheets for these Neoverse V3 datacenter processors.
keywords: ["ARM Silicon", "Arm AGI CPU", "specifications", "data sheet", "datasheet", "Neoverse V3", "AI infrastructure", "datacenter processor"]
description: Explore the ARM AGI CPU family, Arm's first production silicon for AI infrastructure. View specs and datasheets for these Neoverse V3 datacenter processors.
images:
- Arm-Silicon-Header.png
---

# ARM Silicon

While Arm primarily licenses CPU and GPU designs to other manufacturers, they also produce their own silicon for specific datacenter and AI infrastructure applications.

## ARM AGI CPU

![Arm Silicon Hero](Arm-Silicon-Header.png?w=1280&format=webp)


Announced at the Arm Everywhere Keynote on March 24, 2026, the ARM AGI CPU is Arm's first production silicon, designed for AI infrastructure at scale. It delivers a new class of CPU with high performance and extreme rack-level density support for agentic AI operations across modern data centers.

### Specifications

- **Cores:** Up to 136 [Neoverse V3](/docs/soc-manufacturers/arm/#2023) cores (2x 128 SVE, 2MB/core L2)
- **Architecture:** Armv9.2 with bfloat16 and INT8 AI instructions
- **Clock Speed:** Up to 3.7GHz boost
- **PCIe:** 96 Lanes of PCIe Gen6, CXL 3.0 Type 3
- **Process:** 3nm lithography process
- **TDP:** Up to 420W TDP
- **Memory:** Up to 6 Terabyte of DDR5-8800 (12x DDR5 channels)
- **Design:** Dual-Chiplet Design

### SKUs

The ARM AGI CPU is available in three distinct SKUs:

- [**SP113012**](./sp113012/): 136-core flagship model for maximum core count.
- [**SP113012S**](./sp113012s/): 128-core model optimized for Total Cost of Ownership (TCO).
- [**SP113012A**](./sp113012a/): 64-core model optimized for maximum memory bandwidth per core.

### Server Configurations

Arm’s reference server configuration is a 10U, 2-node design – packing in two chips with dedicated memory and I/O for a total of 272 cores per blade. These blades are designed to fully populate a standard air-cooled 36kW rack – 30 blades delivering a total of 8160 cores. 

Arm has additionally partnered with Supermicro on a liquid-cooled 200kW design capable of housing 336 Arm AGI CPUs for over 45,000 cores.

For more information, visit the [official Arm AGI CPU page](https://www.arm.com/products/cloud-datacenter/arm-agi-cpu) or read the [Product Brief](https://www.arm.com/static/az/pdf/product-brief/arm-agi-cpu-product-brief.pdf).
