---
weight: 12
title: Dragonwing Q6 / IQ6
soc-series:
- Dragonwing
soc:
- Q-6690
- QCM6490
- QCS6490
- QCS610
- QCS6125
- IQ-615
tags:
- SOC-Qualcomm
- Dragonwing-Q
summary: Qualcomm Dragonwing Q6 and IQ6. Commercial parts include Q-6690, QCS6490, QCM6490, QCS610, and QCS6125, rated up to 12 TOPS. IQ-615 is the industrial part.
---
# Dragonwing Q6 / IQ6

The Qualcomm Dragonwing Q6 series is the commercial tier for retail, logistics, healthcare, warehousing, and manufacturing. Qualcomm rates that tier at up to 12 TOPS, with Wi-Fi 6E and optional 5G. IQ6 is the industrial tier for HMIs, edge controllers, gateways, handhelds, and machine vision. [QCS6490 / QCM6490](/docs/soc-manufacturers/qualcomm/dragonwing-6490/) has its own page. IQ-615 is the industrial part, with a Kryo 460 cluster of Cortex-A76 and Cortex-A55 cores and a Spectra 230 ISP.

## General Specifications
{{% details title="Specs" open=true %}}

{{< soc-specs >}}

{{% /details %}}

### Variant Differences:

- **Q-6690**: Newer 4 nm part. Two DisplayPort outputs with multi-stream transport. 167 GPIOs.
- **QCS610**: USB 2.0, USB 3.1, and RGMII Ethernet. Two displays. The Cortex-A76 cluster is the same generation as the Talos platform ([SM6150 / QCS615](https://linux-msm.github.io/mainline-status/soc/talos)). QCS610 itself is not listed on that matrix.
- **QCS6125**: Adds the integrated X12 LTE modem that QCS610 does not have.
- **IQ-615**: Industrial grade. Spectra 230, Adreno VPU 443 (4K60 H.265/H.264/VP9 decode, 1080p60 H.265/H.264 encode), up to six cameras, and three displays. RGMII Ethernet, USB, PCIe, and Bluetooth 5.3. Junction temperature is -40°C to 105°C. Qualcomm lists support until 2038.

---

## Linux Support

### Mainline kernel

- **QCS6490 / QCM6490**: Fully supported. Matrix is on the [chip page](/docs/soc-manufacturers/qualcomm/dragonwing-6490/).
- **Q-6690, QCS610, QCS6125, IQ-615**: No mainline status matrix lists these SKUs. QCS610 and IQ-615 use the same Cortex-A76 generation as [Talos (SM6150 / QCS615)](https://linux-msm.github.io/mainline-status/soc/talos).

### Qualcomm Linux

- [x] IQ-615 lists Yocto Linux and Ubuntu

---

## Resources

- [Q6 series](https://www.qualcomm.com/internet-of-things/products/q6-series)
- [IQ6 series](https://www.qualcomm.com/internet-of-things/products/iq6-series)
- [IQ-615](https://www.qualcomm.com/internet-of-things/products/iq6-series/iq-615)
- [Q-6690 product brief](https://docs.qualcomm.com/doc/87-91418-1/87-91418-1_REV_A_Qualcomm_Dragonwing_Q-6690_Processor_Product_Brief.pdf)
- [Product longevity program](https://www.qualcomm.com/internet-of-things/products/product-longevity-program)

---

## Boards with Dragonwing Q6 / IQ6

List of boards:

{{< taglist tag="Q-6690" style="cards" >}}

{{< taglist tag="QCS6490" style="cards" >}}

{{< taglist tag="QCM6490" style="cards" >}}

{{< taglist tag="QCS610" style="cards" >}}

{{< taglist tag="QCS6125" style="cards" >}}

{{< taglist tag="IQ-615" style="cards" >}}
