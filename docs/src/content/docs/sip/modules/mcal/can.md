---
title: "SIP: Can"
sidebar:
  order: 1
---

# SIP: Can

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **Can** (Basic Software – MCAL). Canonical reference: [Can](../../../modules/mcal/can/). Sources: `BSW/Can/`.

## Delivery scope

MICROSAR CAN driver for RH850 (MCAN). MCAL driver implementing the AUTOSAR Can Driver API: controller init, baud-rate handling, transmit/receive, interrupts and wakeup.

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_Can_RH850_MCAN](../../../modules/mcal/can/can-can-rh850-mcan/)

## API snapshot

```c
Can_InitMemory
Can_Init
Can_InitController
Can_ChangeBaudrate
Can_CheckBaudrate
Can_SetBaudrate
Can_InitStruct
Can_GetVersionInfo
```
