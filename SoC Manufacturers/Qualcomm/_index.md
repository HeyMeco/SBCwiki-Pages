---
weight: 10
title: Qualcomm
icon: /assets/qualcomm/Qualcomm-Logo.png
categories:
- soc-vendors
soc-vendors:
- Qualcomm
bookCollapseSection: true
summary: All Qualcomm SoC's, boards, and development resources on sbcwiki.com
---

![Qualcomm Logo](assets/qualcomm/Qualcomm-Logo.png?h=100)

## Summary

Qualcomm designs wireless and computing semiconductors from San Diego, California. For IoT and single-board computers the current brand is **Dragonwing**, with industrial **IQ** parts and commercial **Q** parts. Some of those names are two grades of one SoC. CPUs are Qualcomm Oryon cores, or Arm Cortex designs sold as Kryo. GPUs are [Adreno](./adreno-gpu).

Part numbers use a few prefixes. **QCS** is the application processor without an integrated cellular modem, **QCM** adds that modem, and **QRB** marks robotics parts. Industrial parts are also sold under **IQ-** names, such as IQ-9075 in the IQ9 series. Newer parts use a **Q-** number, such as Q-6690 in the Q6 series.

The lineup below follows Qualcomm's Industrial-Embedded IoT product catalog. Figures are series maxima. Chips in the same series can differ, and product longevity depends on the individual part.

## Dragonwing

Dragonwing is Qualcomm's IoT brand. The IQ series is the industrial line, and the Q series is the commercial line.

{{< taglist Dragonwing-IQ >}}

{{< taglist Dragonwing-Q >}}

## Snapdragon

Snapdragon is Qualcomm's mobile phone SoC, and the brand on its PC processors, including the X Elite, X2 Elite, and 8cx families.

{{< taglist Snapdragon >}}

## Lineup

| Silicon | Grades | Compute | Lifecycle | Target applications |
|---------|--------|---------|-----------|---------------------|
| [IQ10](/docs/soc-manufacturers/qualcomm/dragonwing-iq10/) | Industrial | 350 TOPS, 18-core Oryon. Yocto Linux and Ubuntu | -40°C to 125°C, supported until 2038 | Advanced robotics |
| [Snapdragon X Elite / IQ-X](/docs/soc-manufacturers/qualcomm/snapdragon-x-elite/) | Commercial and industrial. Same Hamoa SoC. IQ-X7181 is the industrial grade of X1E-78-100 | 45 TOPS, up to 12-core Oryon. Windows | IQ-X: -40°C to 105°C, supported until 2036 | Windows PCs, industrial PCs, factory automation, panel PCs, smart displays, surveillance and NVR |
| [IQ9](/docs/soc-manufacturers/qualcomm/dragonwing-iq9/) | Industrial | 100 TOPS, 8-core CPU. Yocto Linux and Ubuntu | -40°C to 115°C, supported until 2038 | Edge AI boxes, robotics, gateways, vision kiosks, machine vision, factory automation, unified HMI and PLC, fleet cameras, surveillance and NVR boxes |
| [Q8 / IQ8](/docs/soc-manufacturers/qualcomm/dragonwing-q8/) | Commercial and industrial. IQ8 is QCS8275 and QCS8300. The commercial parts are separate SoCs, from Q-8750 down to SDA845 | Up to 77 TOPS. Android, Linux, Ubuntu, and Yocto | Q8: -30°C to 105°C, until 2033–2036. IQ8: -40°C to 125°C, until 2038 | Smart displays, conferencing, media devices, fleet cameras, machine vision, gateways, PLCs, and robotics |
| [Q7](/docs/soc-manufacturers/qualcomm/dragonwing-q7/) | Commercial | 24 TOPS, 8-core CPU. Linux and Ubuntu | -30°C to 95°C, supported until 2035 | Smart displays and home hubs, smart appliances, AI TVs and media stations, industrial handhelds, and body and dash cameras |
| [Q6 / IQ6](/docs/soc-manufacturers/qualcomm/dragonwing-q6/) | Commercial and industrial. Includes [QCS6490 / QCM6490](/docs/soc-manufacturers/qualcomm/dragonwing-6490/). IQ-615 is the industrial part | Up to 12 TOPS. Android, Windows, Linux, Ubuntu, and Yocto | Q6: -30°C to 95°C, until 2030–2033. IQ-615: -40°C to 105°C, until 2038 | Retail, logistics, healthcare, warehousing, manufacturing, HMIs, edge controllers, and industrial gateways |
| [Q5](/docs/soc-manufacturers/qualcomm/dragonwing-q5/) | Commercial | 9 TOPS, 8-core CPU. Android, Windows, Linux, and Ubuntu | -30°C to 95°C, supported until 2036 | Ruggedized handhelds, tablets, industrial scanners and HMIs, cameras and edge AI boxes, kiosks and POS systems, and autonomous mobile robots |
| [Q4](/docs/soc-manufacturers/qualcomm/dragonwing-q4/) | Commercial | 1.1 TOPS, 4-core CPU. Android, Linux, and Ubuntu | -30°C to 95°C, supported until 2033–2036 | Industrial handhelds, smart retail, edge AI cameras, industrial computing, healthcare devices, and robotics and automation |
| [Q2 / IQ2](/docs/soc-manufacturers/qualcomm/dragonwing-q2/) | Commercial and industrial. Q-2390 and IQ-2390 are one SoC. QRB2210, QCS2290, and QCM2290 are a Cortex-A53 SoC | Up to 1.1 TOPS. Android, Linux, Ubuntu, and Zephyr | -30°C to 115°C, supported until 2036 | HMIs, small PLCs, machine vision, panels, handhelds, POS, robotics, and entry IoT. QRB2210 is the part on the Arduino Uno Q |

## Qualcomm Adreno GPUs

For more information about Qualcomm Adreno GPU Generations and Drivers check the following subpage: [Adreno-GPU](./adreno-gpu)

## Tutorials

- Coming soon!

{{< taglist TuT-Qualcomm >}}
