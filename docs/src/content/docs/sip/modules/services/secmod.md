---
title: "SIP: SecMod"
sidebar:
  order: 1
---

# SIP: SecMod

![Vector-provided](https://img.shields.io/badge/Vector-provided-blue)

> SIP CBD1800284 view of **SecMod** (Basic Software – Services). Canonical reference: [SecMod](../../../modules/services/secmod/). Sources: `BSW/SecMod/`.

## Delivery scope

Vector Security Module (HIS-compliant Sec + ESLib crypto): CRC, seed/key (Sec_SeedKey), signature verification (Sec_Verification, RSA/RIPEMD-160/act* bignum) for secure boot and secure flashing.

**Origin in this delivery:** Vector-provided.

## SIP documents

- [TechnicalReference_SecurityModule](../../../modules/services/secmod/secmod-securitymodule/)

## API snapshot

```c
esl_initESCryptoLib
esl_initWorkSpaceHeader
esl_initFIPS186
esl_getBytesFIPS186
esl_stirFIPS186
esl_generateKeyAES128
esl_generateKeyAES192
esl_generateKeyAES256
```
