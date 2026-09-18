---
title: "SIP: Crc"
sidebar:
  order: 1
---

# SIP: Crc

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **Crc** (Basic Software – Services). Canonical reference: [Crc](../../../modules/services/crc/). Sources: `BSW/Crc/`.

## Delivery scope

AUTOSAR CRC library: CRC-8/16/32 calculation routines used for data-integrity checks (e.g. NvM, Fee, SecMod verification support).

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_Crc](../../../modules/services/crc/crc-crc/)

## API snapshot

```c
Crc_CalculateCRC8
Crc_CalculateCRC8H2F
Crc_CalculateCRC16
Crc_CalculateCRC32
Crc_CalculateCRC32P4
Crc_CalculateCRC64
Crc_GetVersionInfo
```
