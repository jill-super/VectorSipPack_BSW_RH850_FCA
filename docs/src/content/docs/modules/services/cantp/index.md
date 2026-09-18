---
title: "CanTp"
sidebar:
  order: 1
---

# CanTp
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

AUTOSAR CAN Transport Protocol (ISO 15765-2). Segmentation/reassembly of large diagnostic PDUs over CAN for the bootloader diagnostics path.
## Responsibility

ISO 15765-2 transport for UDS diagnostics flashing (multi-frame reception/transmission).
## Key files

```text
BSW/CanTp/CanTp.c
BSW/CanTp/CanTp.h
BSW/CanTp/CanTp_Cbk.h
BSW/CanTp/CanTp_Priv.h
BSW/CanTp/CanTp_Types.h
```

Browse sources: `BSW/CanTp/`

Build fragments: `mak/CanTp_cfg.mak`, `mak/CanTp_check.mak`, `mak/CanTp_defs.mak`, `mak/CanTp_rules.mak`

## Public API (excerpt from headers)

```c
CanTp_Init
CanTp_InitMemory
CanTp_Shutdown
CanTp_Transmit
CanTp_MainFunction
CanTp_GetVersionInfo
CanTp_ChangeParameter
CanTp_ReadParameter
CanTp_CancelTransmit
CanTp_CancelReceive
CanTp_RxIndication
CanTp_TxConfirmation
CanTp_StopSeparationTime
Appl_CanTpRxSFIndication
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
CanTp_Init(&CanTp_Config);
/* RX indication arrives via CanIf; transmit via PduR_CanTpTransmit */
```

## Dependencies

`CanIf`, `PduR`

## Converted Vector documents

- [TechnicalReference_CanTp](cantp-cantp/) (source: `Doc/TechnicalReferences/TechnicalReference_CanTp.pdf`)

## BSWMD

- `BSWMD/CanTp/CanTp_Pre_bswmd.arxml`
- `BSWMD/CanTp/CanTp_bswmd.arxml`
