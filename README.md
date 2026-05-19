# Pro-Light Node Showcase

![Platform](https://img.shields.io/badge/platform-ESP32_S3-blue)
![Framework](https://img.shields.io/badge/framework-ESP--IDF-green)
![Network](https://img.shields.io/badge/network-BLE_Mesh-orange)
![Status](https://img.shields.io/badge/status-active_development-brightgreen)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

> This repository contains the public-facing architecture, diagnostics workflows, development notes, screenshots, and infrastructure overview for the Pro-Light Node project.
>
> The core firmware and production mesh implementation are currently maintained in a separate private repository while the system architecture is actively evolving.

Pro-Light Node is an ESP32-S3 based BLE Mesh lighting infrastructure project designed for scalable professional lighting systems.

The long-term vision is to create a lightweight, production-oriented lighting ecosystem inspired by professional synchronized lighting platforms such as Sidus Link, while remaining accessible to independent developers, makers, and small production teams.

---

# What This Repository Contains

This public showcase repository includes:

- architecture overview
- development screenshots
- hardware testing evidence
- Android control interface screenshots
- provisioning workflow documentation
- diagnostic workflow notes
- NotebookLM-assisted engineering context
- public roadmap and production goals

This repository does **not** contain the current private firmware source code.

---

# Android Mesh Network Interface

![Network Interface](assets/images/network.jpeg)

Production-oriented Android mesh control interface with:

- real-time node visibility
- RSSI monitoring
- online/offline lifecycle tracking
- mesh diagnostics
- node management workflows

---

# Device Discovery and Provisioning

## Device Discovery

![Provisioning Scan](assets/images/new_device_scan.jpeg)

## Provisioning Workflow

![Provisioning Setup](assets/images/provise_setup.jpeg)

The onboarding architecture focuses on:

- controlled provisioning
- production-safe lifecycle handling
- group assignment
- scalable node management
- future large-scale deployment support

---

# Real-Time RGB Control

![RGB Control](assets/images/color_plate.jpeg)

Low-latency RGB control system supporting:

- group lighting control
- distributed mesh commands
- real-time color workflows
- synchronized lighting behaviors

---

# Effect Engine

![Effect Engine](assets/images/efect.jpeg)

Experimental synchronized effect infrastructure supporting:

- distributed lighting effects
- scheduler-driven execution
- future cue/timeline systems
- coordinated multi-node behavior

---

# Real Hardware Testing

![Hardware Testing](assets/images/real_esp.jpeg)

The project is actively tested on real ESP32-S3 hardware during architecture iteration and mesh reliability development.

Current testing areas include:

- BLE Mesh reliability
- multicast/group delivery behavior
- synchronization workflows
- runtime telemetry
- production-safe node lifecycle handling

---

# Runtime Diagnostic Engine

![Diagnostic Engine](assets/images/diagnostic.png)

Custom runtime diagnostic and packet analysis tooling is used for:

- BLE Mesh lifecycle debugging
- packet inspection
- synchronization analysis
- onboarding diagnostics
- runtime telemetry analysis
- Android + ESP trace correlation
- large-scale reasoning workflows

The diagnostic tooling itself is currently maintained privately while selected public documentation and screenshots are shared here.

---

# Project Goals

- Stable BLE Mesh communication
- Reliable group/unicast command delivery
- Time-synchronized lighting effects
- Production-grade node lifecycle management
- Scalable multi-node lighting architecture
- Real-world hardware testing
- Low-latency lighting control workflows
- Reproducible diagnostics and trace analysis

---

# Architecture Overview

The private firmware is structured around modular embedded subsystems.

```text
src/
 ├── control/
 │    ├── command/
 │    ├── health/
 │    ├── render/
 │    └── safety/
 │
 ├── effects/
 │
 ├── fan/
 │
 ├── hardware/
 │
 ├── mesh/
 │    ├── core/
 │    ├── manager/
 │    └── vendor/
 │
 ├── protocol/
 │
 ├── telemetry/
 │
 ├── thermal/
 │
 └── time_sync/
