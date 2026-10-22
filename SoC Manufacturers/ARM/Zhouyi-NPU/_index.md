---
weight: 3
title: Zhouyi NPU
categories:
- soc-vendors
soc-vendors:
- ARM
keywords: ["Arm-China", "Zhouyi NPU", "Zhouyi Z1", "Zhouyi Z2", "Zhouyi X2", "Zhouyi X3", "AIPU", "Compass", "AI", "NPU", "Machine Learning", "SoC vendors"]
summary: Overview of Arm-China's Zhouyi NPU (AIPU) family, including the Z1, Z2, X2 and X3 generations, the Compass software stack and the SoCs that use it.
bookToc: true
---

# Arm-China Zhouyi NPU

Zhouyi is Arm-China's family of neural processing units, also called AIPUs, licensed to SoC vendors for on-device AI inference. The NPU does not depend on the host CPU architecture, so it is found in both Arm and RISC-V SoCs. It scales from low-power edge designs up to multi-core clusters for high-performance SoCs.

## Key Features

- **Scalability:** From single-core edge configurations up to multi-core clusters.
- **CPU Independent:** Integrates next to Arm or RISC-V host CPUs.
- **Transformer Support:** Zhouyi X2 and later accelerate Transformer-based models, including large language models.
- **Toolchain:** The Zhouyi Compass software stack compiles, quantizes and deploys models from TensorFlow, ONNX and PyTorch.
- **Linux Support:** Open-source kernel driver, proposed for upstreaming into the Linux `accel` subsystem in 2024.

## Generations

| Generation | Year | Notes |
| :--- | :--- | :--- |
| **Zhouyi Z1** | 2018 | Arm-China's first in-house IP, unveiled at the World Internet Conference in Wuzhen |
| **Zhouyi Z2** | 2020 | Mid-to-high-end applications: security, smart cockpits, ADAS and edge servers. Up to 128 TOPS per SoC |
| **Zhouyi X2** | 2023 | Multi-core clusters and Transformer support. Up to 320 TOPS |
| **Zhouyi X3** | 2025 | DSP + DSA design for large model inference. 8 to 80 FP8 TFLOPS per cluster |

## SoCs with Zhouyi NPU

| SoC | NPU Performance |
| :--- | :--- |
| [Cix CD8180 / P1](/docs/soc-manufacturers/cix/cd8180-p1/) | 30 TOPS |
| SiEngine SE1000 | 3.34 TOPS + 3.5 TOPS (two NPU cores, Zhouyi Z2) |
| Allwinner R329 | |

## Software

The Zhouyi Compass software stack is open source and available on [Arm-China's GitHub](https://github.com/Arm-China):

- **[Compass Unified Parser](https://github.com/Arm-China/Compass_Unified_Parser):** Converts models from common frameworks into the Compass float IR.
- **[Compass Optimizer](https://github.com/Arm-China/Compass_Optimizer):** Quantizes the float IR into an optimized quantized or mixed IR for Zhouyi NPUs.
- **[Compass NPU Driver](https://github.com/Arm-China/Compass_NPU_Driver):** Linux kernel driver and runtime for Zhouyi NPUs.
- **[Compass Integration](https://github.com/Arm-China/Compass_Integration):** Integration scripts and examples for the Compass stack.
- **[Compass Apache TVM](https://github.com/Arm-China/Compass_Apache_TVM):** Apache TVM with Zhouyi NPU support for model optimization and heterogeneous execution.
- **[Compass ONNX Runtime](https://github.com/Arm-China/Compass_Onnxruntime):** ONNX Runtime with a Zhouyi NPU execution provider.
- **[Model Zoo](https://github.com/Arm-China/Model_zoo):** Pre-converted models for Zhouyi NPUs.

## Resources

- [Arm-China on GitHub](https://github.com/Arm-China)
- [Radxa SiRider S1 Zhouyi AIPU SDK guide](https://docs.radxa.com/en/sirider/s1/app-development/zhouyi_npu)
- [Phoronix: Arm China upstreaming the Zhouyi NPU driver](https://www.phoronix.com/news/Arm-China-Zhouyi-NPU-Linux-RFC)
