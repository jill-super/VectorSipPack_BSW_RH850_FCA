---
title: "SecMod"
sidebar:
  order: 1
---

# SecMod
![Vector-provided](https://img.shields.io/badge/Vector-provided-blue) ![Layer](https://img.shields.io/badge/layer-services-lightgrey)
> **Origin:** Vector-provided. Proprietary Vector MICROSAR code — keep the Vector copyright header; governed by the Vector license terms, not MIT.
## Purpose

Vector Security Module (HIS-compliant Sec + ESLib crypto): CRC, seed/key (Sec_SeedKey), signature verification (Sec_Verification, RSA/RIPEMD-160/act* bignum) for secure boot and secure flashing.
## Responsibility

HIS security services: hashing, signatures, seed/key and secure verification for boot and flashing.
## Key files

```text
BSW/SecMod/ESLib.h
BSW/SecMod/ESLib_ASN_1.h
BSW/SecMod/ESLib_Config.h
BSW/SecMod/ESLib_ERC.h
BSW/SecMod/ESLib_Init.c
BSW/SecMod/ESLib_RMD160.c
BSW/SecMod/ESLib_RNG.h
BSW/SecMod/ESLib_RSA_V15_EM.c
BSW/SecMod/ESLib_RSA_V15_Ver_RIPEMD160.c
BSW/SecMod/ESLib_RSAprim_ver.c
BSW/SecMod/ESLib_V1.1_compatibility.h
BSW/SecMod/ESLib_t.h
BSW/SecMod/ESLib_types.h
BSW/SecMod/ESLib_version.c
BSW/SecMod/ESLib_version.h
BSW/SecMod/Sec.c
BSW/SecMod/Sec.h
BSW/SecMod/SecM.h
BSW/SecMod/SecM_Inc.h
BSW/SecMod/Sec_Crc.c
BSW/SecMod/Sec_Crc.h
BSW/SecMod/Sec_Inc.h
BSW/SecMod/Sec_SeedKey.c
BSW/SecMod/Sec_SeedKey.h
BSW/SecMod/Sec_Types.h
BSW/SecMod/Sec_Verification.c
BSW/SecMod/Sec_Verification.h
BSW/SecMod/Sec_VerificationLib.c
BSW/SecMod/Sec_VerificationLib.h
BSW/SecMod/Sec_Workspace.h
```

(59 source files in total; generated/Config files excluded above.)

Browse sources: `BSW/SecMod/`

Build fragments: `mak/SecMod_cfg.mak`, `mak/SecMod_check.mak`, `mak/SecMod_defs.mak`, `mak/SecMod_rules.mak`

## Public API (excerpt from headers)

```c
esl_initESCryptoLib
esl_initWorkSpaceHeader
esl_initFIPS186
esl_getBytesFIPS186
esl_stirFIPS186
esl_generateKeyAES128
esl_generateKeyAES192
esl_generateKeyAES256
esl_initEncryptAES128
esl_initEncryptAES192
esl_initEncryptAES256
esl_encryptAES128
esl_encryptAES192
esl_encryptAES256
```

Full signatures live in the headers listed above; the Vector Technical Reference is authoritative for call sequences and constraints.

## Usage example

```c
SecM_Init();
if (SecM_Verify(/* hash/signature over image */) == SEC_OK) { /* boot */ }
```

## Dependencies

`Crc`, `Det`, `Fbl`

## Converted Vector documents

- [TechnicalReference_SecurityModule](secmod-securitymodule/) (source: `Doc/TechnicalReferences/TechnicalReference_SecurityModule.pdf`)
