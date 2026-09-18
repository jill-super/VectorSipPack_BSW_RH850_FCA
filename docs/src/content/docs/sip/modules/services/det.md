---
title: "SIP: Det"
sidebar:
  order: 1
---

# SIP: Det

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **Det** (Basic Software – Services). Canonical reference: [Det](../../../modules/services/det/). Sources: `BSW/Det/`.

## Delivery scope

AUTOSAR Default Error Tracer. Central development-error reporting hook (Det_ReportError / ReportRuntimeError / ReportTransientFault) used by all MICROSAR modules.

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_Det](../../../modules/services/det/det-det/)

## API snapshot

```c
Det_Init
Det_Start
Det_InitMemory
Det_ReportError
Det_ReportRuntimeError
Det_ReportTransientFault
Det_GetVersionInfo
```
