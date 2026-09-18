---
title: "Can"
sidebar:
  order: 1
---

# Can
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-mcal-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

MICROSAR CAN driver for RH850 (MCAN). MCAL driver implementing the AUTOSAR Can Driver API: controller init, baud-rate handling, transmit/receive, interrupts and wakeup.
## Responsibility

Low-level CAN controller access for all TX/RX in bootloader and updater contexts, including wakeup handling.
## Key files

```text
BSW/Can/Can.c
BSW/Can/Can.h
BSW/Can/Can_Irq.c
BSW/Can/Can_Local.h
```

Browse sources: `BSW/Can/`

Build fragments: `mak/Can_cfg.mak`, `mak/Can_check.mak`, `mak/Can_defs.mak`, `mak/Can_rules.mak`

## Public API (excerpt from headers)

```c
Can_InitMemory
Can_Init
Can_InitController
Can_ChangeBaudrate
Can_CheckBaudrate
Can_SetBaudrate
Can_InitStruct
Can_GetVersionInfo
Can_GetStatus
Can_SetControllerMode
Can_ResetBusOffStart
Can_ResetBusOffEnd
Can_Write
Can_CancelTx
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`_Common`, `Det`, `CanIf (upper layer)`

## Converted Vector documents

- [TechnicalReference_Can_RH850_MCAN](can-can-rh850-mcan/) (source: `Doc/TechnicalReferences/TechnicalReference_Can_RH850_MCAN.pdf`)

## BSWMD

- `BSWMD/Can/Can_Mpc5700Mcan_bswmd.arxml`
- `BSWMD/CanIf/CanIf_Pre_bswmd.arxml`
- `BSWMD/CanIf/CanIf_bswmd.arxml`
- `BSWMD/CanTp/CanTp_Pre_bswmd.arxml`
- `BSWMD/CanTp/CanTp_bswmd.arxml`
