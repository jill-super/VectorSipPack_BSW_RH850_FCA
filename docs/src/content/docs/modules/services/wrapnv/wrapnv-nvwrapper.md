---
title: "Converted: WrapNv (NvWrapper)"
sidebar:
  order: 2
---

# Converted: Technical Reference — WrapNv (NvWrapper)

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_NvWrapper.pdf` — 27 pages · original title `NV-Wrapper`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **WrapNv (NvWrapper)**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- NV-Wrapper
- Technical Reference
- Wrapper for non-volatile memory access
- Status Released
- Technical Reference NV-Wrapper
- Document Information
- History
- Author Date Version Remarks
- Reference Documents
- Caution
- Contents
- 4.1.1.2 Synchronous API ................................ ........................... 13
- 4.1.1.2.1 WrapNv_ReadSync ................................ ... 13
- 4.1.1.2.2 WrapNv_ReadPartialSync ......................... 14

## Key content (extracted text sample)

NV-Wrapper 
Technical Reference 
 
Wrapper for non-volatile memory access 
Version 2.02 
 
 
 
 
 
 
 
 
 
 
 
Authors Christian Bäuerle, Achim Strobelt, Marco Riedl 
Status Released 
 
 
 
 
 
Technical Reference NV-Wrapper 
© 2017 Vector Informatik GmbH Version 2.02 2 
based on template version 4.11.3 
Document Information 
History 
Author Date Version Remarks 
Christian Bäuerle 2009-09-19 0.90 Initial Draft 
Achim Strobelt 2012-01-26 1.00 Configuration with GENy 
Marco Riedl 2016-03-02 2.00 Added Fee/NvM 
Marco Riedl 2016-03-20 2.01 Changed API 
Marco Riedl 2017-06-29 2.02 Added Ea 
Reference Documents 
No. Source Title Version 
[1] Vector Flash Bootloader User Manual 2.7 
[2] Vector EEPROM Manager, Technical Reference 1.3 
[3] Vector Flash Driver Wrapper, Technical Reference 1.1 
 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 

Technical Reference NV-Wrapper 
© 2017 Vector Informatik GmbH Version 2.02 3 
based on template version 4.11.3 
Contents 
1 Introduction................................ ................................ ................................ ................... 6 
2 Functional Description ................................ ................................ ................................ . 7 
2.1 Architecture ................................ ................................ ................................ ........ 7 
2.2 Data structures ................................ ................................ ................................ .. 8 
2.2.1 Single ................................ ................................ ................................ . 8 
2.2.2 List ................................ ................................ ................................ ..... 8 
2.2.3 Structure ................................ ................................ ............................ 8 
2.2.4 Table ................................ ................................ ................................ .. 8 
2.3 NV-Wrapper in Application ................................ ................................ ................. 8 
3 Integration ................................ ................................ ................................ ................... 10 
3.1 Scope of delivery ................................ ................................ ............................. 10 
3.1.1 Core files ................................ ................................ .......................... 10 
3.1.2 Application files ................................ ................................ ................ 10 
3.1.3 Generated files ................................ ................................ ................. 11 
3.2 Include structure ................................ ................................ .............................. 11 
3.2.1 Initialization ................................ ................................ ...................... 11 
3.2.2 Memory accesses ................................ ................................ ............ 12 
4 API Description ................................ ................................ ................................ ........... 13 
4.1 Function API ................................ ................................ ................................ .... 13 
4.1.1 Function Description ................................ ................................ ........ 13 
4.1.1.1 WrapNv_Init ................................ ................................ ... 13 
4.1.1.2 Synchronous API ................................ ........................... 13 
4.1.1.2.1 WrapNv_ReadSync ................................ ... 13 
4.1.1.2.2 WrapNv_ReadPartialSync ......................... 14 
4.1.1.2.3 WrapNv_WriteSync ................................ .... 14 
4.1.1.2.4 WrapNv_DeleteSync ................................ .. 15 
4.1.1.3 Asynchronous API ................................ ......................... 15 
4.1.1.3.1 WrapNv_ReadAsync ................................ .. 15 
4.1.1.3.2 WrapNv_ReadPartialAsync ........................ 16 
4.1.1.3.3 WrapNv_WriteAsync ................................ .. 17 
4.1.1.3.4 WrapNv_DeleteAsync ................................ 17 
4.2 Naming […]

## Related module

See [WrapNv](../) for purpose, API, files and dependencies.
