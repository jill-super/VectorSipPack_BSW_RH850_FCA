---
title: "SIP: FblAsrStubs"
sidebar:
  order: 1
---

# SIP: FblAsrStubs

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **FblAsrStubs** (Complex Device Drivers (CDD)). Canonical reference: [FblAsrStubs](../../../modules/cdd/fblasrstubs/). Sources: `BSW/FblAsrStubs/`.

## Delivery scope

Bootloader-environment stubs for AUTOSAR modules absent in the FBL context (EcuM, ComM, Dem, Os/Rte, SchM). Lets FBL reuse ASR BSW (CanIf/CanTp/PduR/NvM) without a full ECU stack.

**Origin in this delivery:** Vector-provided.

## API snapshot

```c
ComM_BusSM_ModeIndication
Dem_ReportErrorStatus
EcuM_SetWakeupEvent
EcuM_CheckWakeup
Can_MainFunction_Write
Can_MainFunction_BusOff
Can_MainFunction_Read
Can_MainFunction_Wakeup
```
