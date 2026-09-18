---
title: "Det"
sidebar:
  order: 1
---

# Det
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

AUTOSAR Default Error Tracer. Central development-error reporting hook (Det_ReportError / ReportRuntimeError / ReportTransientFault) used by all MICROSAR modules.
## Responsibility

Development error tracer; stub/disable for production, keep active during integration testing.
## Key files

```text
BSW/Det/Det.c
BSW/Det/Det.h
```

Browse sources: `BSW/Det/`

Build fragments: `mak/Det_cfg.mak`, `mak/Det_check.mak`, `mak/Det_defs.mak`, `mak/Det_rules.mak`

## Public API (excerpt from headers)

```c
Det_Init
Det_Start
Det_InitMemory
Det_ReportError
Det_ReportRuntimeError
Det_ReportTransientFault
Det_GetVersionInfo
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
Det_Init(&Det_Config);
(void)Det_ReportError(MODULE_ID, INSTANCE_ID, API_ID, ERROR_ID);
```

## Dependencies

`_Common`

## Converted Vector documents

- [TechnicalReference_Det](det-det/) (source: `Doc/TechnicalReferences/TechnicalReference_Det.pdf`)

## BSWMD

- `BSWMD/Det/Det_Pre_bswmd.arxml`
- `BSWMD/Det/Det_bswmd.arxml`
