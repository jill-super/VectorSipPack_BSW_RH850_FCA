---
title: "Converted: FBL FCA (OEM)"
sidebar:
  order: 2
---

# Converted: Technical Reference — FBL FCA (OEM)

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_FBL_Fca.pdf` — 78 pages · original title `Flash Bootloader OEM`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **FBL FCA (OEM)**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- Technical Reference Flash Bootloader OEM
- Flash Bootloader OEM
- Technical Reference
- Status Not Released
- Document Information
- History
- Author Date Version Remarks
- Reference Documents
- Caution
- Contents
- 5.2.3.1 Memory Device Table ................................ .................... 22
- 5.2.3.2 Flash Block Table ................................ ........................... 22
- 5.2.3.3 Logical Block Table ................................ ........................ 23
- 5.2.3.4 NV-Wrapper Configuration ................................ ............. 24

## Key content (extracted text sample)

Technical Reference Flash Bootloader OEM 
© 2018 Vector Informatik GmbH Version 0.9 1 
based on template version 5.1.0 
 
 
 
 
 
 
 
 
 
 
 
 
Flash Bootloader OEM 
Technical Reference 
 
FCA UDS (SLP5) 
Version 0.9 
 
 
 
 
 
 
 
 
 
 
Authors Christian Bäuerle 
Status Not Released 
 
 
 
 
 
Technical Reference Flash Bootloader OEM 
© 2018 Vector Informatik GmbH Version 0.9 2 
based on template version 5.1.0 
Document Information 
History 
Author Date Version Remarks 
Christian Bäuerle 2018-07-12 0.9 Creation 
 
 
Technical Reference Flash Bootloader OEM 
© 2018 Vector Informatik GmbH Version 0.9 3 
based on template version 5.1.0 
Reference Documents 
No. Source Title Version 
[1] ISO 14229 Road Vehicles – Unified diagnostic services (UDS) 
Part 1: Specification and Requirements 
2013 
[2] ISO 15765 Road Vehicles – Diagnostics on CAN 
Part 3: Implementation of Unified Diagnostic Services 
2004 
[3] Vector AN-ISC-8-1188 – Custom Flash Drivers 1.0 
[4] HIS Security Module Specification 1.0 
[5] Vector User Manual Flash Bootloader 2.7 
[6] Vector Technical Reference HexView 1.12.2 
[7] Vector Manual vFlash 3.5 
[8] Vector NV-Wrapper – Technical Reference 1.0 
[9] Vector AN-ISC-8-1143 – Bootloader Validation Strategies 1.0 
[10] Vector Technical Reference Security Module / Security Module Basic 2.2.0 
[11] Vector AN-ISC-8-1188 – Custom Flash Drivers 1.0 
[12] Vector Technical Reference Communication Wrapper PDU Router 3.2 
[13] FCA CS.00100 Comprehensive Standard Unified Diagnostic Services 
(UDS) On CAN 
2016-
12-07 
[14] FCA CS.00101 ECU Flash Reprogramming Requirements - UDS 2018-
03-23 
[15] FCA CS.00102 Standardized Diagnostic Data 2016-
12-07 
 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 

Technical Reference Flash Bootloader OEM 
© 2018 Vector Informatik GmbH Version 0.9 4 
based on template version 5.1.0 
Contents 
1 Introduction................................ ................................ ................................ ................... 8 
2 Download concept ................................ ................................ ................................ ........ 9 
2.1 Overview ................................ ................................ ................................ ............ 9 
3 Flash Bootloader Delivery ................................ ................................ .......................... 10 
3.1 Bootloader Components ................................ ................................ .................. 10 
3.2 Bootloader Integration ................................ ................................ ...................... 10 
4 Bootloader Installation ................................ ................................ ............................... 12 
4.1 [#oem_files] - Bootloader package structure ................................ .................... 12 
4.2 Demonstration Bootloader ................................ ................................ ............... 14 
5 Generation Tool (DaVinci Configurator 5) ................................ ................................ . 15 
5.1 Project Setup and Communication Stack Configuration ................................ ... 15 
5.2 Bootloader Configuration ................................ ................................ ................. 16 
5.2.1 General Bootloader Options ................................ ............................. 16 
5.2.2 OEM Bootloader Options ................................ ................................ . 21 
5.2.3 Memory Configuration ................................ ................................ ...... 22 
5.2.3.1 Memory Device Table ................................ .................... 22 
5.2.3.2 Flash Block Table ................................ ........................... 22 
5.2.3.3 Logical Block Table ................................ ........................ 23 
5.2.3.4 NV-Wrapper Configuration ................................ ............. 24 
5.2.4 Security Module Configuration ................................ ......................... 26 
5.2.4.1 Check Routine Without Additional CRC and Without 
Additional Signature ................................ ....................... 26 […]

## Related module

See [Fbl](../) for purpose, API, files and dependencies.
