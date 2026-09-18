---
title: "Fee_30_SmallSector"
sidebar:
  order: 1
---

# Fee_30_SmallSector
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

MICROSAR Flash EEPROM Emulation (SmallSector variant): block-oriented non-volatile storage on top of the flash driver, with dataset/instance/partition handlers and task manager.
## Responsibility

Owns emulated-EEPROM block persistence used by NvM/WrapNv.
## Key files

```text
BSW/Fee_30_SmallSector/Fee_30_SmallSector.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_BlockHandler.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_BlockHandler.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Cbk.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_DatasetHandler.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_DatasetHandler.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_FlsCoordinator.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_FlsCoordinator.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_InstanceHandler.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_InstanceHandler.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer1_Read.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer1_Read.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer1_Write.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer1_Write.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer2_DatasetEraser.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer2_DatasetEraser.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer2_InstanceFinder.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer2_InstanceFinder.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer2_WriteInstance.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer2_WriteInstance.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer3_ReadManagementBytes.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_Layer3_ReadManagementBytes.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_PartitionHandler.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_PartitionHandler.h
BSW/Fee_30_SmallSector/Fee_30_SmallSector_TaskManager.c
BSW/Fee_30_SmallSector/Fee_30_SmallSector_TaskManager.h
```

Browse sources: `BSW/Fee_30_SmallSector/`

Build fragments: `mak/Fee_30_SmallSector_cfg.mak`, `mak/Fee_30_SmallSector_check.mak`, `mak/Fee_30_SmallSector_defs.mak`, `mak/Fee_30_SmallSector_rules.mak`

## Public API (excerpt from headers)

```c
Fee_30_SmallSector_Init
Fee_30_SmallSector_Read
Fee_30_SmallSector_Write
Fee_30_SmallSector_InvalidateBlock
Fee_30_SmallSector_EraseImmediateBlock
Fee_30_SmallSector_Cancel
Fee_30_SmallSector_GetStatus
Fee_30_SmallSector_GetJobResult
Fee_30_SmallSector_GetVersionInfo
Fee_30_SmallSector_SetMode
Fee_30_SmallSector_SuspendWrites
Fee_30_SmallSector_ResumeWrites
Fee_30_SmallSector_MainFunction
Fee_30_SmallSector_AlignValue
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`MemIf`, `Det`, `Flash (via Fls)`

## Converted Vector documents

- [TechnicalReference_Fee_30_SmallSector](fee_30_smallsector-fee-30-smallsector/) (source: `Doc/TechnicalReferences/TechnicalReference_Fee_30_SmallSector.pdf`)

## BSWMD

- `BSWMD/Fee_30_SmallSector/Fee_30_SmallSector_bswmd_Asr4.0.3.arxml`
