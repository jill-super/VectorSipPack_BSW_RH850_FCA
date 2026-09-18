---
title: "Flash"
sidebar:
  order: 1
---

# Flash
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-cdd-lightgrey)
> **Origin:** Vector-provided (generated artifacts: Custom/generated). Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

RH850 flash programming support: flashdrv (Vector flash driver for RH850/RV40) plus generated FlashRom C-array (HexView output) and GHS build files in Build/.
## Responsibility

Owns on-chip flash primitives and the generated flash-driver ROM image.
## Key files

```text
BSW/Flash/FlashRom.c
BSW/Flash/FlashRom.h
BSW/Flash/flashdrv.c
BSW/Flash/flashdrv.h
```

Browse sources: `BSW/Flash/`

## Public API (excerpt from headers)

No exported C API surface detected (types/macros/templates only) — see headers and templates in the file list.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`Fbl`, `FblUpd`

## Converted Vector documents

No dedicated Technical Reference in this SIP slice — see the FBL/peer module documents.

## BSWMD

- `BSWMD/Fbl/FblOem_Flash_RH850_Pre.arxml`
