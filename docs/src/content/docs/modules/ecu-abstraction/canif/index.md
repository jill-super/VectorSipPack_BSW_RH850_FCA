---
title: "CanIf"
sidebar:
  order: 1
---

# CanIf
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-ecu-abstraction-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

AUTOSAR CAN Interface: ECU-abstraction layer multiplexing PDU traffic between the CAN driver (Can) and upper layers (CanTp, PduR, FblCw).
## Responsibility

Single ECU-abstraction entry point for CAN traffic; routes between driver and PduR/CanTp/FblCw.
## Key files

```text
BSW/CanIf/CanIf.c
BSW/CanIf/CanIf.h
BSW/CanIf/CanIf_Cbk.h
BSW/CanIf/CanIf_GeneralTypes.h
BSW/CanIf/CanIf_Hooks.h
BSW/CanIf/CanIf_Types.h
```

Browse sources: `BSW/CanIf/`

## Public API (excerpt from headers)

```c
CanIf_InitMemory
CanIf_Init
CanIf_SetControllerMode
CanIf_GetControllerMode
CanIf_Transmit
CanIf_SetPduMode
CanIf_GetPduMode
CanIf_GetVersionInfo
CanIf_SetTrcvMode
CanIf_GetTrcvMode
CanIf_GetTrcvWakeupReason
CanIf_SetTrcvWakeupMode
CanIf_TrcvModeIndication
CanIf_ConfirmPnAvailability
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`Can`, `PduR`, `CanTp`

## Converted Vector documents

- [TechnicalReference_CanIf](canif-canif/) (source: `Doc/TechnicalReferences/TechnicalReference_CanIf.pdf`)

## BSWMD

- `BSWMD/CanIf/CanIf_Pre_bswmd.arxml`
- `BSWMD/CanIf/CanIf_bswmd.arxml`
