---
title: "_Common"
sidebar:
  order: 1
---

# _Common
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-common-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

Shared MICROSAR platform headers: Std_Types, Platform_Types, Compiler (+ _Compiler_Cfg), ComStack_Types, MemMap_Common/_MemMap and v_def. Included by every BSW module.
## Responsibility

Shared type/compiler/memory-mapping foundation for the whole SIP.
## Key files

```text
BSW/_Common/Can_GeneralTypes.h
BSW/_Common/ComStack_Types.h
BSW/_Common/Compiler.h
BSW/_Common/MemMap_Common.h
BSW/_Common/Platform_Types.h
BSW/_Common/Std_Types.h
BSW/_Common/_Compiler_Cfg.h
BSW/_Common/_MemMap.h
BSW/_Common/v_def.h
```

Browse sources: `BSW/_Common/`

## Public API (excerpt from headers)

```c
rettype
EccSedNotif_print
EccDedNotif_print
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

None (foundation module).

## Converted Vector documents

- [TechnicalReference_Asr_MemoryMapping](shared-asr-memorymapping/) (source: `Doc/TechnicalReferences/TechnicalReference_Asr_MemoryMapping.pdf`)
- [TechnicalReference_ComStackLib](shared-comstacklib/) (source: `Doc/TechnicalReferences/TechnicalReference_ComStackLib.pdf`)
