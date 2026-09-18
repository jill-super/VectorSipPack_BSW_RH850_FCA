---
title: "WrapNv"
sidebar:
  order: 1
---

# WrapNv
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

Vector Nv Wrapper: bootloader-side abstraction over NvM/Fee/Fls/Ea/EEL (WrapNv.c + generated _WrapNv_Cfg), so FBL application code accesses NV memory uniformly.
## Responsibility

Bootloader-friendly NV access facade over NvM/Fee/Fls.
## Key files

```text
BSW/WrapNv/WrapNv.c
BSW/WrapNv/WrapNv.h
BSW/WrapNv/_WrapNv_Cfg.c
BSW/WrapNv/_WrapNv_Cfg.h
BSW/WrapNv/_WrapNv_inc.h
```

Browse sources: `BSW/WrapNv/`

## Public API (excerpt from headers)

```c
WrapNv_Init
WrapNv_ReadSync
WrapNv_ReadPartialSync
WrapNv_WriteSync
WrapNv_DeleteSync
WrapNv_ReadAsync
WrapNv_ReadPartialAsync
WrapNv_WriteAsync
WrapNv_DeleteAsync
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
WrapNv_Init();
WrapNv_ReadSync(recordId, buffer);  /* facade over NvM/Fee */
```

## Dependencies

`NvM`, `Fee_30_SmallSector`, `MemIf`

## Converted Vector documents

- [TechnicalReference_NvWrapper](wrapnv-nvwrapper/) (source: `Doc/TechnicalReferences/TechnicalReference_NvWrapper.pdf`)

## BSWMD

- `BSWMD/WrapNv/WrapNv_Pre_bswmd.arxml`
