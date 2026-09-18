---
title: "FblAsrStubs"
sidebar:
  order: 1
---

# FblAsrStubs
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-cdd-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

Bootloader-environment stubs for AUTOSAR modules absent in the FBL context (EcuM, ComM, Dem, Os/Rte, SchM). Lets FBL reuse ASR BSW (CanIf/CanTp/PduR/NvM) without a full ECU stack.
## Responsibility

Provides EcuM/ComM/Dem/Os/SchM stand-ins so ASR BSW links inside the bootloader.
## Key files

```text
BSW/FblAsrStubs/ComM.h
BSW/FblAsrStubs/ComM_BusSM.h
BSW/FblAsrStubs/ComM_Types.h
BSW/FblAsrStubs/Dem.c
BSW/FblAsrStubs/Dem.h
BSW/FblAsrStubs/EcuM.c
BSW/FblAsrStubs/EcuM.h
BSW/FblAsrStubs/EcuM_Cbk.h
BSW/FblAsrStubs/EcuM_Generated_Types.h
BSW/FblAsrStubs/FblAsrStubs.h
BSW/FblAsrStubs/Os.h
BSW/FblAsrStubs/Rte.h
BSW/FblAsrStubs/Rte_ComM.h
BSW/FblAsrStubs/Rte_ComM_Type.h
BSW/FblAsrStubs/Rte_EcuM_Type.h
BSW/FblAsrStubs/Rte_NvM_Type.h
BSW/FblAsrStubs/Rte_Type.h
BSW/FblAsrStubs/SchM_Can.h
BSW/FblAsrStubs/SchM_CanIf.h
BSW/FblAsrStubs/SchM_CanTp.h
BSW/FblAsrStubs/SchM_Det.h
BSW/FblAsrStubs/SchM_Fee.h
BSW/FblAsrStubs/SchM_Fls.h
BSW/FblAsrStubs/SchM_NvM.h
BSW/FblAsrStubs/SchM_NvM_Type.h
BSW/FblAsrStubs/SchM_PduR.h
BSW/FblAsrStubs/SchM_WrapNv.h
```

Browse sources: `BSW/FblAsrStubs/`

## Public API (excerpt from headers)

```c
ComM_BusSM_ModeIndication
Dem_ReportErrorStatus
EcuM_SetWakeupEvent
EcuM_CheckWakeup
Can_MainFunction_Write
Can_MainFunction_BusOff
Can_MainFunction_Read
Can_MainFunction_Wakeup
Can_MainFunction_Mode
CanTp_MainFunction
Fls_MainFunction
FblInterruptDisable
NvM_MainFunction
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`CanIf`, `CanTp`, `PduR`, `NvM`

## Converted Vector documents

No dedicated Technical Reference in this SIP slice — see the FBL/peer module documents.
