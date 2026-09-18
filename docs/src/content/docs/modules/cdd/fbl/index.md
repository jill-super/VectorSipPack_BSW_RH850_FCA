---
title: "Fbl"
sidebar:
  order: 1
---

# Fbl
![Vector-provided, FCA-customised](https://img.shields.io/badge/Vector-provided,%20FCA-customised-purple) ![Layer](https://img.shields.io/badge/layer-cdd-lightgrey)
> **Origin:** Vector-provided, FCA-customised. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

Vector Flash Bootloader core (FBL FCA variant for SLP5): startup, memory programming, UDS diagnostics (fbl_diag_core + OEM diagnostics), flash interaction (fbl_mem, fbl_flio), watchdog handling and application validation/boot.
## Responsibility

Owns the bootloader lifecycle: reset entry → validation → diagnostics/programming → boot jump.
## Key files

```text
BSW/Fbl/applvect.h
BSW/Fbl/fbl_applvect.c
BSW/Fbl/fbl_assert.h
BSW/Fbl/fbl_assert_oem.h
BSW/Fbl/fbl_def.h
BSW/Fbl/fbl_diag.h
BSW/Fbl/fbl_diag_core.c
BSW/Fbl/fbl_diag_core.h
BSW/Fbl/fbl_diag_oem.c
BSW/Fbl/fbl_diag_oem.h
BSW/Fbl/fbl_flio.c
BSW/Fbl/fbl_flio.h
BSW/Fbl/fbl_hw.c
BSW/Fbl/fbl_hw.h
BSW/Fbl/fbl_main.c
BSW/Fbl/fbl_main.h
BSW/Fbl/fbl_mem.c
BSW/Fbl/fbl_mem.h
BSW/Fbl/fbl_mem_oem.h
BSW/Fbl/fbl_mio.c
BSW/Fbl/fbl_mio.h
BSW/Fbl/fbl_sfr.h
BSW/Fbl/fbl_vect.c
BSW/Fbl/fbl_wd.c
BSW/Fbl/fbl_wd.h
BSW/Fbl/iotypes.h
BSW/Fbl/v_ver.h
```

Browse sources: `BSW/Fbl/`

## Public API (excerpt from headers)

```c
FblDiagDefaultPostHandler
FblDiagOem_ProcessDeclineRequest
FblReadBlock
FblReadByte
FblMemInitPowerOn
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
/* Entry: FblMain() dispatches tasks; OEM hooks live in Demo/DemoFbl/Appl/Source/fbl_ap*.c */
FblMain();
```

## Dependencies

`FblCw`, `FblBm`, `SecMod`, `WrapNv`, `Flash`, `MemMap/_Common`

## Converted Vector documents

- [TechnicalReference_FBL_Fca](fbl-fbl-fca/) (source: `Doc/TechnicalReferences/TechnicalReference_FBL_Fca.pdf`)
- [TechnicalReference_FBL_RH850](fbl-fbl-rh850/) (source: `Doc/TechnicalReferences/TechnicalReference_FBL_RH850.pdf`)

## BSWMD

- `BSWMD/Fbl/FblOem_Fca_bswmd.arxml`
- `BSWMD/Fbl/FblOem_Fca_bswmd_Pre.arxml`
- `BSWMD/Fbl/FblOem_Flash_RH850_Pre.arxml`
- `BSWMD/FblCw/FblCw_Fca_Pre_bswmd.arxml`
- `BSWMD/FblHal/FblHal_Rh850_P1M-C_GreenHills_Pre_bswmd.arxml`
- `BSWMD/FblHal/FblHal_Rh850_bswmd.arxml`
