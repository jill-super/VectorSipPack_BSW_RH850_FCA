---
title: "NvM"
sidebar:
  order: 1
---

# NvM
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

AUTOSAR NVRAM Manager: RAM-mirror/block management, job queuing (JobProc/Queue), CRC handling and callbacks on top of MemIf/Fee.
## Responsibility

Manages NV blocks, RAM mirrors and asynchronous job processing.
## Key files

```text
BSW/NvM/NvM.c
BSW/NvM/NvM.h
BSW/NvM/NvM_Act.c
BSW/NvM/NvM_Act.h
BSW/NvM/NvM_Cbk.h
BSW/NvM/NvM_Crc.c
BSW/NvM/NvM_Crc.h
BSW/NvM/NvM_JobProc.c
BSW/NvM/NvM_JobProc.h
BSW/NvM/NvM_Qry.c
BSW/NvM/NvM_Qry.h
BSW/NvM/NvM_Queue.c
BSW/NvM/NvM_Queue.h
BSW/NvM/NvM_Types.h
```

Browse sources: `BSW/NvM/`

Build fragments: `mak/NvM_cfg.mak`, `mak/NvM_check.mak`, `mak/NvM_defs.mak`, `mak/NvM_rules.mak`

## Public API (excerpt from headers)

```c
NvM_Init
NvM_SetDataIndex
NvM_GetDataIndex
NvM_SetBlockProtection
NvM_GetErrorStatus
NvM_GetVersionInfo
NvM_SetRamBlockStatus
NvM_ReadBlock
NvM_WriteBlock
NvM_RestoreBlockDefaults
NvM_EraseNvBlock
NvM_InvalidateNvBlock
NvM_CancelJobs
NvM_ReadAll
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
NvM_Init();
NvM_ReadBlock(blockId, ramMirrorPtr);  /* async — poll NvM_GetErrorStatus */
```

## Dependencies

`MemIf`, `Fee_30_SmallSector`, `Crc`, `Det`

## Converted Vector documents

- [TechnicalReference_NvM](nvm-nvm/) (source: `Doc/TechnicalReferences/TechnicalReference_NvM.pdf`)

## BSWMD

- `BSWMD/NvM/NvM_bswmd.arxml`
