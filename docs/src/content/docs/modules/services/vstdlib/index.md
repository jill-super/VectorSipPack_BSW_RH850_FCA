---
title: "VStdLib"
sidebar:
  order: 1
---

# VStdLib
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

Vector Standard Library: optimised memset/memcpy and helpers (vstdlib) shared by all MICROSAR modules.
## Responsibility

Shared low-level helpers with deterministic behaviour for all BSW.
## Key files

```text
BSW/VStdLib/_VStdLib_Cfg.h
BSW/VStdLib/vstdlib.c
BSW/VStdLib/vstdlib.h
```

Browse sources: `BSW/VStdLib/`

Build fragments: `mak/VStdLib_cfg.mak`, `mak/VStdLib_check.mak`, `mak/VStdLib_defs.mak`, `mak/VStdLib_rules.mak`

## Public API (excerpt from headers)

```c
VStdLib_MemSet
VStdLib_MemCpy
VStdLib_MemCpy16
VStdLib_MemCpy32
VStdLib_MemCpy_s
VStdLib_GetVersionInfo
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`_Common`

## Converted Vector documents

- [TechnicalReference_VStdLib_GenericAsr](vstdlib-vstdlib-genericasr/) (source: `Doc/TechnicalReferences/TechnicalReference_VStdLib_GenericAsr.pdf`)
