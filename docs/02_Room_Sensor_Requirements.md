# Requirements Specification

## Introduction

This document defines the functional and non-functional requirements for the first Hugin room sensor.

The requirements serve as the basis for implementation, testing and validation.

---

# Functional Requirements

## FR-001 Human Presence Detection

The device shall detect human presence using an mmWave sensor.

### Acceptance Criteria

- Detect moving occupants.
- Detect stationary occupants.
- Presence state shall be reported automatically to Home Assistant.

---

## FR-002 Temperature Measurement

The device shall measure ambient temperature.

### Acceptance Criteria

- Temperature shall be reported to Home Assistant.
- Measurement values shall be updated automatically within Home Assistant.

---

## FR-003 Relative Humidity Measurement

The device shall measure relative humidity.

### Acceptance Criteria

- Humidity shall be reported to Home Assistant.
- Measurement values shall be updated automatically within Home Assistant.

---

## FR-004 Ambient Light Measurement

The device shall measure ambient illuminance.

### Acceptance Criteria

- Illuminance shall be reported in lux.
- Measurement values shall be updated automatically within Home Assistant.

---

## FR-005 Local Operation

The device shall operate without requiring Internet connectivity.

### Acceptance Criteria

- All functionality shall remain available on the local network.
- No cloud services shall be required.

---

## FR-006 Home Assistant Integration

The device shall integrate with Home Assistant using ESPHome.

### Acceptance Criteria

- The device shall be discoverable by Home Assistant.
- Sensor entities shall be automatically available within Home Assistant.
- OTA firmware updates shall be supported.

---

## FR-007 Power

The device shall be powered via USB-C.

### Acceptance Criteria

- The device shall operate continuously while externally powered.

---

## FR-008 Configuration

The device shall support configuration through ESPHome.

### Acceptance Criteria

- Configuration shall be stored within the ESPHome configuration.
- No custom firmware modifications shall be required for normal operation.

---

# Non-Functional Requirements

## NFR-001 Reliability

The device shall automatically recover after power loss and reconnect to the local Wi-Fi network without manual intervention.

---

## NFR-002 Maintainability

The hardware and firmware shall be documented sufficiently to allow the sensor to be reproduced by another developer.

---

## NFR-003 Modularity

Future Hugin sensor variants shall be able to reuse the same hardware and software architecture where practical.

---

## NFR-004 Documentation

All hardware revisions, firmware revisions and significant design decisions shall be documented within this repository.

---

## Out of Scope

The following functionality is not included in Version 1.0:

- Battery operation
- Matter support
- Bluetooth Proxy
- Display
- CO₂ measurement
- Mobile application