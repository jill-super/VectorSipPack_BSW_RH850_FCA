---
title: "SIP: CanTp"
sidebar:
  order: 1
---

# SIP: CanTp

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **CanTp** (Basic Software – Services). Canonical reference: [CanTp](../../../modules/services/cantp/). Sources: `BSW/CanTp/`.

## Delivery scope

AUTOSAR CAN Transport Protocol (ISO 15765-2). Segmentation/reassembly of large diagnostic PDUs over CAN for the bootloader diagnostics path.

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_CanTp](../../../modules/services/cantp/cantp-cantp/)

## API snapshot

```c
CanTp_Init
CanTp_InitMemory
CanTp_Shutdown
CanTp_Transmit
CanTp_MainFunction
CanTp_GetVersionInfo
CanTp_ChangeParameter
CanTp_ReadParameter
```
