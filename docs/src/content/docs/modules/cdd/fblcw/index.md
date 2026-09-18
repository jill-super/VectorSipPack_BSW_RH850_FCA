---
title: "FblCw"
sidebar:
  order: 1
---

# FblCw
![Vector-provided, FCA-customised](https://img.shields.io/badge/Vector-provided,%20FCA-customised-purple) ![Layer](https://img.shields.io/badge/layer-cdd-lightgrey)
> **Origin:** Vector-provided, FCA-customised. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

FBL Communication Wrapper: thin CAN-oriented communication layer (fbl_cw) connecting the bootloader diagnostics to CanIf/PduR/CanTp, FCA-customised (FblCw_Fca).
## Responsibility

Owns bootloader-side CAN communication adaptation toward CanIf/PduR.
## Key files

```text
BSW/FblCw/fbl_cw.c
BSW/FblCw/fbl_cw.h
```

Browse sources: `BSW/FblCw/`

## Public API (excerpt from headers)

```c
FblCw_InitMemory
FblCw_Init
FblCw_Deinit
FblCw_ChangeParameter
FblCw_ResetParameter
FblCw_ReadParameter
Dcm_ComM_NoComModeEntered
Dcm_ComM_SilentComModeEntered
Dcm_ComM_FullComModeEntered
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`CanIf`, `PduR`, `CanTp`, `Fbl`

## Converted Vector documents

- [TechnicalReference_FblCw](fblcw-fblcw/) (source: `Doc/TechnicalReferences/TechnicalReference_FblCw.pdf`)

## BSWMD

- `BSWMD/FblCw/FblCw_Fca_Pre_bswmd.arxml`
