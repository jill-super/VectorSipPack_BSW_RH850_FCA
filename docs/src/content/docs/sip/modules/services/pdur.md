---
title: "SIP: PduR"
sidebar:
  order: 1
---

# SIP: PduR

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **PduR** (Basic Software – Services). Canonical reference: [PduR](../../../modules/services/pdur/). Sources: `BSW/PduR/`.

## Delivery scope

AUTOSAR PDU Router: routes I-PDUs between CanIf, CanTp, Dcm/FblCw and the bootloader (incl. FblBm routing variant PduR_Bm).

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_PduR](../../../modules/services/pdur/pdur-pdur/)

## API snapshot

```c
PduR_GetConfigurationId
PduR_Init
PduR_InitMemory
PduR_GetVersionInfo
PduR_UpTransmit
PduR_LoIfRxIndication
PduR_LoIfTriggerTransmit
PduR_LoIfTxConfirmation
```
