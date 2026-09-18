---
title: "SIP: BswM"
sidebar:
  order: 1
---

# SIP: BswM

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **BswM** (Basic Software – Services). Canonical reference: [BswM](../../../modules/services/bswm/). Sources: `BSW/BswM/`.

## Delivery scope

AUTOSAR Basic Software Mode Manager (MICROSAR BswM). Arbitrates mode requests from application, ComM, DCM, EcuM and other BSW, evaluates arbitration rules and executes mode-switch actions.

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_BswM](../../../modules/services/bswm/bswm-bswm/)

## API snapshot

```c
BswM_InitMemory
BswM_Init
BswM_Deinit
BswM_GetVersionInfo
BswM_RequestMode
BswM_RuleControl
BswM_CanSM_CurrentState
BswM_ComM_CurrentMode
```
