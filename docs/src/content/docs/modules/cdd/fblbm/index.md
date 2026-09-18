---
title: "FblBm"
sidebar:
  order: 1
---

# FblBm
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-cdd-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

FBL Boot Manager: decides at reset whether to stay in the bootloader or jump to the application (boot conditions, target handling). Used by the DemoBm example and FCA startup flow.
## Responsibility

Owns the stay-in-boot vs. jump-to-application decision.
## Key files

```text
BSW/FblBm/fbl_bm.c
BSW/FblBm/fbl_bm.h
BSW/FblBm/fbl_bmtypes.h
```

Browse sources: `BSW/FblBm/`

## Public API (excerpt from headers)

No exported C API surface detected (types/macros/templates only) — see headers and templates in the file list.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`Fbl`

## Converted Vector documents

No dedicated Technical Reference in this SIP slice — see the FBL/peer module documents.
