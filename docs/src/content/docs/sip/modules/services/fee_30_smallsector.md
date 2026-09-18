---
title: "SIP: Fee_30_SmallSector"
sidebar:
  order: 1
---

# SIP: Fee_30_SmallSector

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **Fee_30_SmallSector** (Basic Software – Services). Canonical reference: [Fee_30_SmallSector](../../../modules/services/fee_30_smallsector/). Sources: `BSW/Fee_30_SmallSector/`.

## Delivery scope

MICROSAR Flash EEPROM Emulation (SmallSector variant): block-oriented non-volatile storage on top of the flash driver, with dataset/instance/partition handlers and task manager.

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_Fee_30_SmallSector](../../../modules/services/fee_30_smallsector/fee_30_smallsector-fee-30-smallsector/)

## API snapshot

```c
Fee_30_SmallSector_Init
Fee_30_SmallSector_Read
Fee_30_SmallSector_Write
Fee_30_SmallSector_InvalidateBlock
Fee_30_SmallSector_EraseImmediateBlock
Fee_30_SmallSector_Cancel
Fee_30_SmallSector_GetStatus
Fee_30_SmallSector_GetJobResult
```
