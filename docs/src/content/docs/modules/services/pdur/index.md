---
title: "PduR"
sidebar:
  order: 1
---

# PduR
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

AUTOSAR PDU Router: routes I-PDUs between CanIf, CanTp, Dcm/FblCw and the bootloader (incl. FblBm routing variant PduR_Bm).
## Responsibility

Routes PDUs between CanIf/CanTp and Dcm/FblCw (plus Boot-Manager variant).
## Key files

```text
BSW/PduR/PduR.c
BSW/PduR/PduR.h
BSW/PduR/PduR_Bm.c
BSW/PduR/PduR_Bm.h
```

Browse sources: `BSW/PduR/`

Build fragments: `mak/PduR_cfg.mak`, `mak/PduR_check.mak`, `mak/PduR_defs.mak`, `mak/PduR_rules.mak`

## Public API (excerpt from headers)

```c
PduR_GetConfigurationId
PduR_Init
PduR_InitMemory
PduR_GetVersionInfo
PduR_UpTransmit
PduR_LoIfRxIndication
PduR_LoIfTriggerTransmit
PduR_LoIfTxConfirmation
PduR_LoTpStartOfReception
PduR_LoTpCopyRxData
PduR_LoTpRxIndication
PduR_LoTpCopyTxData
PduR_LoTpTxConfirmation
PduR_CancelReceive
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
PduR_Init(&PduR_Config);
PduR_CanTpTransmit(txPduId, &pduInfo);  /* routed to CanIf/CanTp per config */
```

## Dependencies

`CanIf`, `CanTp`, `FblCw`

## Converted Vector documents

- [TechnicalReference_PduR](pdur-pdur/) (source: `Doc/TechnicalReferences/TechnicalReference_PduR.pdf`)

## BSWMD

- `BSWMD/PduR/PduR_Pre_bswmd.arxml`
- `BSWMD/PduR/PduR_bswmd.arxml`
