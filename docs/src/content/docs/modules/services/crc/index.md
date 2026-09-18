---
title: "Crc"
sidebar:
  order: 1
---

# Crc
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

AUTOSAR CRC library: CRC-8/16/32 calculation routines used for data-integrity checks (e.g. NvM, Fee, SecMod verification support).
## Responsibility

Deterministic CRC services for NvM/Fee integrity and verification helpers.
## Key files

```text
BSW/Crc/Crc.c
BSW/Crc/Crc.h
```

Browse sources: `BSW/Crc/`

Build fragments: `mak/Crc_cfg.mak`, `mak/Crc_check.mak`, `mak/Crc_defs.mak`, `mak/Crc_rules.mak`

## Public API (excerpt from headers)

```c
Crc_CalculateCRC8
Crc_CalculateCRC8H2F
Crc_CalculateCRC16
Crc_CalculateCRC32
Crc_CalculateCRC32P4
Crc_CalculateCRC64
Crc_GetVersionInfo
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
uint32 crc = Crc_CalculateCRC32(data, len, 0u, TRUE);
```

## Dependencies

`_Common`

## Converted Vector documents

- [TechnicalReference_Crc](crc-crc/) (source: `Doc/TechnicalReferences/TechnicalReference_Crc.pdf`)

## BSWMD

- `BSWMD/Crc/Crc_bswmd.arxml`
