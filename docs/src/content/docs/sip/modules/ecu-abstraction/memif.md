---
title: "SIP: MemIf"
sidebar:
  order: 1
---

# SIP: MemIf

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **MemIf** (Basic Software – ECU Abstraction). Canonical reference: [MemIf](../../../modules/ecu-abstraction/memif/). Sources: `BSW/MemIf/`.

## Delivery scope

AUTOSAR Memory Abstraction Interface: ECU-abstraction router between NvM and the underlying Fee/Ea memory drivers.

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_MemIf](../../../modules/ecu-abstraction/memif/memif-memif/)

## API snapshot

```c
MemIf_Read
MemIf_Write
MemIf_InvalidateBlock
MemIf_EraseImmediateBlock
MemIf_Cancel
MemIf_GetStatus
MemIf_GetJobResult
MemIf_SetMode
```
