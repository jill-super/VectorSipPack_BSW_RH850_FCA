---
title: "SIP: Fbl"
sidebar:
  order: 1
---

# SIP: Fbl

![Vector-provided, FCA-customised](https://img.shields.io/badge/Vector-provided,%20FCA-customised-purple)

> SIP CBD1800284 view of **Fbl** (Complex Device Drivers (CDD)). Canonical reference: [Fbl](../../../modules/cdd/fbl/). Sources: `BSW/Fbl/`.

## Delivery scope

Vector Flash Bootloader core (FBL FCA variant for SLP5): startup, memory programming, UDS diagnostics (fbl_diag_core + OEM diagnostics), flash interaction (fbl_mem, fbl_flio), watchdog handling and application validation/boot.

**Origin in this delivery:** Vector-provided, FCA-customised.

## SIP documents

- [TechnicalReference_FBL_Fca](../../../modules/cdd/fbl/fbl-fbl-fca/)
- [TechnicalReference_FBL_RH850](../../../modules/cdd/fbl/fbl-fbl-rh850/)

## API snapshot

```c
FblDiagDefaultPostHandler
FblDiagOem_ProcessDeclineRequest
FblReadBlock
FblReadByte
FblMemInitPowerOn
```
