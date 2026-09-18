---
title: "Converted: FBL RH850"
sidebar:
  order: 2
---

# Converted: Technical Reference — FBL RH850

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_FBL_RH850.pdf` — 23 pages · original title `Flash Bootloader Hardware`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **FBL RH850**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- Flash Bootloader Hardware
- TechnicalReference
- CANfbl Renesas RH850
- Status Released
- TechnicalReference Flash Bootloader Hardware
- Document Information
- History
- Author Date Version Remarks
- Table 1-1  History of the Document
- Reference Documents
- EALC-SD-1045-
- Table 1-2  References Documents
- Contents
- 3.3.1.2 Channel Settings for Pipelined Programming ................................ .. 16

## Key content (extracted text sample)

Flash Bootloader Hardware 
TechnicalReference 
 
CANfbl Renesas RH850 
 
 
Version 1.00.01 
 
 
 
 
 
 
 
Authors Christian Bäuerle; Robert Schäffner 
Status Released 
 
 
 
 
 
 
TechnicalReference Flash Bootloader Hardware 
2015, Vector Informatik GmbH Version: 1.00.01 
based on template version 3.2.0 
2 / 23 
Document Information 
History 
Author Date Version Remarks 
Christian Bäuerle 2013-06-12 01.00.00 Creation 
Robert Schäffner 2015-05-29 01.00.01 Removed template parts 
Table 1-1 History of the Document 
Reference Documents 
No. Source Title Document No. Version 
[1] Renesas RH850/F1L Group User’s manual 
[2] Renesas V850E3v5 Architecture Specifications 
[3] Renesas T01 - Self-Programming Library for 
Code Flash (RV40 Flash) 
EALC-SD-1045-
1E00b 
 
Table 1-2 References Documents 
 
TechnicalReference Flash Bootloader Hardware 
2015, Vector Informatik GmbH Version: 1.00.01 
based on template version 3.2.0 
3 / 23 
Contents 
1 Introduction ................................ ................................ ................................ .................... 6 
1.1 Configurations covered by this Technical Reference ................................ ....... 6 
1.1.1 Microcontrollers ................................ ................................ ............................... 6 
1.2 Compilers ................................ ................................ ................................ ........ 6 
2 Memory Model ................................ ................................ ................................ ................ 7 
2.1 [#hw_mem] - Design the Memory Layout ................................ ........................ 7 
2.2 Memory Mapping ................................ ................................ ............................ 7 
2.2.1 Memory mapping of application and FBL ................................ ........................ 7 
2.2.2 Memory range of the FBL ................................ ................................ ................ 7 
2.2.3 Memory range of the application ................................ ................................ ..... 8 
2.2.4 Bootloader Sections ................................ ................................ ........................ 8 
2.2.5 Compiler-/Linker specific memory mapping issues ................................ .......... 9 
2.3 [#hw_intvect] - The Interrupt Vector Tables ................................ ...................... 9 
2.3.1 Bootloader Vector Table ................................ ................................ ................ 10 
2.3.2 Application Vector Table ................................ ................................ ................ 10 
2.3.3 Vector base address registers ................................ ................................ ....... 11 
2.3.4 Special measures for NMI ................................ ................................ ............. 11 
3 Hardware Layer ................................ ................................ ................................ ............ 12 
3.1 Flash Memory and Flash Driver ................................ ................................ .... 12 
3.1.1 Special clock parameters and clock settings................................ .................. 12 
3.1.2 Flash Code Buffer Size ................................ ................................ ................. 12 
3.1.3 ID Authentication ................................ ................................ ........................... 12 
3.1.4 Rebuilding the flash driver binary ................................ ................................ .. 13 
3.2 [#hw_size] - Flash Segment Size ................................ ................................ .. 14 
3.3 CAN Driver ................................ ................................ ................................ .... 14 
3.3.1 CAN Channels ................................ ................................ .............................. 14 
3.3.1.1 Number of Supported Channels ................................ ...................... 15 
3.3.1.2 Channel Settings for Pipelined Programming ................................ .. 16 
3.3.2 Sleep Mode ................................ ................................ ................................ ... 16 
3.4 Timer ................................ ................................ ................................ ............. 16 
3.5 Startup Code ................................ ................................ […]

## Related module

See [Fbl](../) for purpose, API, files and dependencies.
