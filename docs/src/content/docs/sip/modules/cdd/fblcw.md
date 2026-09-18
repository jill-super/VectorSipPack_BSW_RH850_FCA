---
title: "SIP: FblCw"
sidebar:
  order: 1
---

# SIP: FblCw

![Vector-provided, FCA-customised](https://img.shields.io/badge/Vector-provided,%20FCA-customised-purple)

> SIP CBD1800284 view of **FblCw** (Complex Device Drivers (CDD)). Canonical reference: [FblCw](../../../modules/cdd/fblcw/). Sources: `BSW/FblCw/`.

## Delivery scope

FBL Communication Wrapper: thin CAN-oriented communication layer (fbl_cw) connecting the bootloader diagnostics to CanIf/PduR/CanTp, FCA-customised (FblCw_Fca).

**Origin in this delivery:** Vector-provided, FCA-customised.

## SIP documents

- [TechnicalReference_FblCw](../../../modules/cdd/fblcw/fblcw-fblcw/)

## API snapshot

```c
FblCw_InitMemory
FblCw_Init
FblCw_Deinit
FblCw_ChangeParameter
FblCw_ResetParameter
FblCw_ReadParameter
Dcm_ComM_NoComModeEntered
Dcm_ComM_SilentComModeEntered
```
