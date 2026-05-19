# Pro-Light Node

![Platform](https://img.shields.io/badge/platform-ESP32_S3-blue)
![Framework](https://img.shields.io/badge/framework-ESP--IDF-green)
![Network](https://img.shields.io/badge/network-BLE_Mesh-orange)
![Status](https://img.shields.io/badge/status-active_development-brightgreen)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

Pro-Light Node is an ESP32-S3 based BLE Mesh lighting node firmware designed for scalable professional lighting systems.

The project focuses on building a lightweight, production-oriented embedded mesh infrastructure for resource-constrained devices using ESP-IDF and Bluetooth Mesh Vendor Models.

The long-term vision is to create a robust open-source lighting ecosystem inspired by professional systems such as Sidus Link while remaining accessible to independent developers and makers.

---

# Android Mesh Network Interface

![Network Interface](assets/images/network.jpeg)

Production-oriented Android mesh control interface with:

* real-time node visibility
* RSSI monitoring
* online/offline lifecycle tracking
* mesh diagnostics
* node management workflows

---

# Device Discovery and Provisioning

### Device Discovery

![Provisioning Scan](assets/images/new_device_scan.jpeg)

### Provisioning Workflow

![Provisioning Setup](assets/images/provise_setup.jpeg)

The onboarding architecture focuses on:

* controlled provisioning
* production-safe lifecycle handling
* group assignment
* scalable node management
* future large-scale deployment support

---

# Real-Time RGB Control

![RGB Control](assets/images/color_plate.jpeg)

Low-latency RGB control system supporting:

* group lighting control
* distributed mesh commands
* real-time color workflows
* synchronized lighting behaviors

---

# Effect Engine

![Effect Engine](assets/images/efect.jpeg)

Experimental synchronized effect infrastructure supporting:

* distributed lighting effects
* scheduler-driven execution
* future cue/timeline systems
* coordinated multi-node behavior

---

# Real Hardware Testing

![Hardware Testing](assets/images/real_esp.jpeg)

The project is actively tested on real ESP32-S3 hardware during architecture iteration and mesh reliability development.

Current testing areas include:

* BLE Mesh reliability
* multicast/group delivery behavior
* synchronization workflows
* runtime telemetry
* production-safe node lifecycle handling

---

# Runtime Diagnostic Engine

![Diagnostic Engine](assets/images/diagnostic.png)

Custom runtime diagnostic and packet analysis tooling used for:

* BLE Mesh lifecycle debugging
* packet inspection
* synchronization analysis
* onboarding diagnostics
* runtime telemetry analysis
* Android + ESP trace correlation
* large-scale reasoning workflows

---

# Goals

* Stable BLE Mesh communication
* Reliable group/unicast command delivery
* Time-synchronized lighting effects
* Production-grade node lifecycle management
* Scalable multi-node lighting architecture
* Real-world hardware testing
* Low-latency lighting control workflows

---

# Core Subsystems

## Mesh Infrastructure

* `mesh/core`
  BLE Mesh initialization and transport layer.

* `mesh/vendor`
  Vendor model packet handling and runtime communication.

* `mesh/manager`
  Node lifecycle and mesh coordination management.

---

## Protocol Infrastructure

* `ProLightProtocolDecoder`
  Protocol abstraction and packet decoding infrastructure.

* `protocol/`
  Runtime command interpretation and protocol workflows.

---

## Command + Scheduler Systems

* `LightCommandScheduler`
  Distributed scheduled command execution infrastructure.

* `LightCommandProcessor`
  Runtime command execution pipeline.

* `LightCommandQueue`
  Command buffering and execution ordering.

---

## Runtime Safety + Health

* `LightRuntimeHealth`
  Runtime health monitoring subsystem.

* `LightSafety`
  Production-oriented command validation and safety controls.

* `TelemetryBridge`
  Runtime telemetry and diagnostics integration layer.

---

## Synchronization Infrastructure

* `TimeSyncManager`
  Experimental synchronization system for coordinated multi-node execution.

---

# Repository Structure

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
```

---

# Structured Diagnostic Workflows

The repository also includes structured engineering and diagnostic resources under:

```text
notebooklm_sources/
```

These resources contain:

* Android lifecycle traces
* provisioning flow documentation
* protocol analysis notes
* synchronization debugging workflows
* ESP runtime diagnostics
* telemetry reasoning references
* architecture context bundles

The goal is to support reproducible debugging and large-scale system reasoning during embedded mesh infrastructure development.

---

# Tech Stack

* ESP32-S3
* ESP-IDF
* PlatformIO
* Bluetooth Mesh
* Vendor Models
* FreeRTOS
* Kotlin Android
* BLE GATT
* Custom Vendor Protocols

---

# Development Philosophy

This project prioritizes:

* stability over shortcuts
* architecture over temporary fixes
* real hardware validation
* reproducible debugging
* production-oriented infrastructure
* maintainable subsystem separation

---

# Project Status

Active development.

The repository is currently under rapid architecture iteration and real hardware testing.

Main ongoing areas:

* mesh reliability
* synchronization systems
* telemetry infrastructure
* distributed scheduling
* node lifecycle management
* production diagnostics

---

# Roadmap

## Phase 1 — Core Stability

* [x] BLE Mesh vendor communication
* [x] Group command support
* [x] Unicast command support
* [x] RGB lighting control
* [x] Master dimmer support
* [x] Real hardware testing

---

## Phase 2 — Protocol Infrastructure

* [x] Protocol decoder layer
* [x] Command scheduling system
* [x] Time synchronization experiments
* [x] Telemetry bridge foundation

---

## Phase 3 — Production Architecture

* [ ] Reliable multi-node synchronization
* [ ] Production-grade online/offline detection
* [ ] Scheduler safety improvements
* [ ] Structured diagnostics
* [ ] Node recovery strategies
* [ ] Mesh congestion handling

---

## Phase 4 — Advanced Lighting Infrastructure

* [ ] Scene engine
* [ ] Cue timeline system
* [ ] Distributed synchronized effects
* [ ] Large-scale node orchestration
* [ ] Mobile control integration

---

# License

MIT License


> This repository is the public documentation, architecture, diagnostics, and development showcase for Pro-Light Node.  
> Core firmware implementation is currently developed in a private repository and will be open-sourced progressively as the architecture stabilizes.
