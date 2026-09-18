---
title: "FblUpd"
sidebar:
  order: 1
---

# FblUpd
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-cdd-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

FBL Updater (programming-session updater): minimal self-update component (upd_main) that reprograms the bootloader itself via templates in _Template.
## Responsibility

Owns in-field bootloader self-update sequencing.
## Key files

```text
BSW/FblUpd/upd_main.c
BSW/FblUpd/upd_main.h
BSW/FblUpd/upd_types.h
```

Browse sources: `BSW/FblUpd/`

## Public API (excerpt from headers)

No exported C API surface detected (types/macros/templates only) — see headers and templates in the file list.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`Fbl`, `Flash`

## Converted Vector documents

- [TechnicalReference_FBL_Updater](fblupd-fbl-updater/) (source: `Doc/TechnicalReferences/TechnicalReference_FBL_Updater.pdf`)
- [TechnicalReference_FBL_Updater_RH850](fblupd-fbl-updater-rh850/) (source: `Doc/TechnicalReferences/TechnicalReference_FBL_Updater_RH850.pdf`)
