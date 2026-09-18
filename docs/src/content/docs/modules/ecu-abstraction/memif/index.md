---
title: "MemIf"
sidebar:
  order: 1
---

# MemIf
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-ecu-abstraction-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

AUTOSAR Memory Abstraction Interface: ECU-abstraction router between NvM and the underlying Fee/Ea memory drivers.
## Responsibility

Routes NvM memory jobs to Fee (or Ea) devices.
## Key files

```text
BSW/MemIf/MemIf.c
BSW/MemIf/MemIf.h
BSW/MemIf/MemIf_Types.h
```

Browse sources: `BSW/MemIf/`

Build fragments: `mak/MemIf_cfg.mak`, `mak/MemIf_check.mak`, `mak/MemIf_defs.mak`, `mak/MemIf_rules.mak`

## Public API (excerpt from headers)

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

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
MemIf_Read(deviceIndex, blockNumber, offset, buffer, length);
```

## Dependencies

`Fee_30_SmallSector`, `NvM`

## Converted Vector documents

- [TechnicalReference_MemIf](memif-memif/) (source: `Doc/TechnicalReferences/TechnicalReference_MemIf.pdf`)

## BSWMD

- `BSWMD/MemIf/MemIf_bswmd.arxml`
