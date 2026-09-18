---
title: "SIP: WrapNv"
sidebar:
  order: 1
---

# SIP: WrapNv

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **WrapNv** (Basic Software – Services). Canonical reference: [WrapNv](../../../modules/services/wrapnv/). Sources: `BSW/WrapNv/`.

## Delivery scope

Vector Nv Wrapper: bootloader-side abstraction over NvM/Fee/Fls/Ea/EEL (WrapNv.c + generated _WrapNv_Cfg), so FBL application code accesses NV memory uniformly.

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_NvWrapper](../../../modules/services/wrapnv/wrapnv-nvwrapper/)

## API snapshot

```c
WrapNv_Init
WrapNv_ReadSync
WrapNv_ReadPartialSync
WrapNv_WriteSync
WrapNv_DeleteSync
WrapNv_ReadAsync
WrapNv_ReadPartialAsync
WrapNv_WriteAsync
```
