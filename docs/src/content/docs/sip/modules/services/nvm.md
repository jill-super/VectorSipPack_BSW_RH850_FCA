---
title: "SIP: NvM"
sidebar:
  order: 1
---

# SIP: NvM

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **NvM** (Basic Software – Services). Canonical reference: [NvM](../../../modules/services/nvm/). Sources: `BSW/NvM/`.

## Delivery scope

AUTOSAR NVRAM Manager: RAM-mirror/block management, job queuing (JobProc/Queue), CRC handling and callbacks on top of MemIf/Fee.

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_NvM](../../../modules/services/nvm/nvm-nvm/)

## API snapshot

```c
NvM_Init
NvM_SetDataIndex
NvM_GetDataIndex
NvM_SetBlockProtection
NvM_GetErrorStatus
NvM_GetVersionInfo
NvM_SetRamBlockStatus
NvM_ReadBlock
```
