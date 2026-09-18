---
title: "BswM"
sidebar:
  order: 1
---

# BswM
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

AUTOSAR Basic Software Mode Manager (MICROSAR BswM). Arbitrates mode requests from application, ComM, DCM, EcuM and other BSW, evaluates arbitration rules and executes mode-switch actions.
## Responsibility

Mode arbitration across the ECU: collects `BswM_RequestMode` calls, evaluates rules and triggers mode-switch actions (e.g. communication control, PduR routing states).
## Key files

```text
BSW/BswM/BswM.c
BSW/BswM/BswM.h
BSW/BswM/BswM_CanSM.h
BSW/BswM/BswM_ComM.h
BSW/BswM/BswM_Dcm.h
BSW/BswM/BswM_EcuM.h
BSW/BswM/BswM_EthIf.h
BSW/BswM/BswM_EthSM.h
BSW/BswM/BswM_FrSM.h
BSW/BswM/BswM_J1939Dcm.h
BSW/BswM/BswM_J1939Nm.h
BSW/BswM/BswM_LinSM.h
BSW/BswM/BswM_LinTp.h
BSW/BswM/BswM_Nm.h
BSW/BswM/BswM_NvM.h
BSW/BswM/BswM_PduR.h
BSW/BswM/BswM_Sd.h
BSW/BswM/BswM_WdgM.h
```

Browse sources: `BSW/BswM/`

Build fragments: `mak/BswM_cfg.mak`, `mak/BswM_check.mak`, `mak/BswM_defs.mak`, `mak/BswM_rules.mak`

## Public API (excerpt from headers)

```c
BswM_InitMemory
BswM_Init
BswM_Deinit
BswM_GetVersionInfo
BswM_RequestMode
BswM_RuleControl
BswM_CanSM_CurrentState
BswM_ComM_CurrentMode
BswM_ComM_InitiateReset
BswM_ComM_CurrentPNCMode
BswM_Dcm_CommunicationMode_CurrentState
BswM_Dcm_ApplicationUpdated
BswM_EcuM_CurrentState
BswM_EcuM_CurrentWakeup
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
BswM_Init(&BswM_Config);
BswM_RequestMode(myUser, MODE_FLASH_SESSION);
```

## Dependencies

`Det`, `EcuM-stub (FblAsrStubs)`, `SchM stubs`

## Converted Vector documents

- [TechnicalReference_BswM](bswm-bswm/) (source: `Doc/TechnicalReferences/TechnicalReference_BswM.pdf`)

## BSWMD

- `BSWMD/BswM/BswM_bswmd.arxml`
- `BSWMD/Can/Can_Mpc5700Mcan_bswmd.arxml`
- `BSWMD/CanIf/CanIf_Pre_bswmd.arxml`
- `BSWMD/CanIf/CanIf_bswmd.arxml`
- `BSWMD/CanTp/CanTp_Pre_bswmd.arxml`
- `BSWMD/CanTp/CanTp_bswmd.arxml`
- `BSWMD/Crc/Crc_bswmd.arxml`
- `BSWMD/Det/Det_Pre_bswmd.arxml`
