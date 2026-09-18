---
title: "SIP: CanIf"
sidebar:
  order: 1
---

# SIP: CanIf

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **CanIf** (Basic Software – ECU Abstraction). Canonical reference: [CanIf](../../../modules/ecu-abstraction/canif/). Sources: `BSW/CanIf/`.

## Delivery scope

AUTOSAR CAN Interface: ECU-abstraction layer multiplexing PDU traffic between the CAN driver (Can) and upper layers (CanTp, PduR, FblCw).

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_CanIf](../../../modules/ecu-abstraction/canif/canif-canif/)

## API snapshot

```c
CanIf_InitMemory
CanIf_Init
CanIf_SetControllerMode
CanIf_GetControllerMode
CanIf_Transmit
CanIf_SetPduMode
CanIf_GetPduMode
CanIf_GetVersionInfo
```
