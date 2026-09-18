---
title: "Converted: Crc"
sidebar:
  order: 2
---

# Converted: Technical Reference — Crc

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_Crc.pdf` — 23 pages · original title `MICROSAR CRC`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **Crc**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR CRC
- Technical Reference
- Status Released
- Technical Reference MICROSAR CRC
- Document Information
- History
- Author Date Version Remarks
- Changed versioning to new notation
- Add Crc8 calculation
- Add Crc8H2F calculation
- Add Crc32P4 calculation
- Reference Documents
- Scope of the Document
- Caution

## Key content (extracted text sample)

MICROSAR CRC 
Technical Reference 
 
 
Version 4.03.00 
 
 
 
 
 
 
 
 
 
 
 
Authors Michael Goß 
Status Released 
 
 
 
 
 
Technical Reference MICROSAR CRC 
© 2016 Vector Informatik GmbH Version 4.03.00 2 
based on template version 5.9.0 
Document Information 
History 
Author Date Version Remarks 
Tobias Schmid 2006-12-13 1.0 Initial Version 
Tobias Schmid 2008-01-21 3.00.00 Update to ASR 2.1 
Changed versioning to new notation 
Claudia Mausz 2008-05-19 4.00.00 Update to ASR 3 
Add Crc8 calculation 
Michael Goß 2014-11-18 4.01.00 Update to ASR 4 
Add Crc8H2F calculation 
Michael Goß 2015-05-08 4.02.00 SafeBSW 
Add Crc32P4 calculation 
Michael Goß 2016-11-24 4.03.00 Add Crc64 calculation 
Reference Documents 
No. Source Title Version 
[1] AUTOSAR AUTOSAR_SWS_CRCLibrary.pdf V4.2.0 
[2] AUTOSAR AUTOSAR_SWS_CRCLibrary.pdf V4.3.0 
[3] AUTOSAR AUTOSAR_TR_BSWModuleList.pdf V1.6.0 
Scope of the Document 
This technical reference describes the general use of the CRC library basis software. 
There are no aspects which are controller specific. 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 

Technical Reference MICROSAR CRC 
© 2016 Vector Informatik GmbH Version 4.03.00 3 
based on template version 5.9.0 
Contents 
1 Component History ................................ ................................ ................................ ...... 6 
2 Introduction................................ ................................ ................................ ................... 7 
2.1 Architecture Overview ................................ ................................ ........................ 8 
3 Functional Description ................................ ................................ ................................ . 9 
3.1 Features ................................ ................................ ................................ ............ 9 
3.1.1 Deviations ................................ ................................ .......................... 9 
3.1.2 Additions/ Extensions ................................ ................................ ....... 10 
3.2 Initialization ................................ ................................ ................................ ...... 10 
3.3 States ................................ ................................ ................................ .............. 10 
3.4 Main Functions ................................ ................................ ................................ 10 
3.5 Error Handling ................................ ................................ ................................ .. 10 
3.5.1 Development Error Reporting ................................ ........................... 10 
3.5.2 Production Code Error Reporting ................................ ..................... 10 
3.5.3 Parameter Checking ................................ ................................ ........ 10 
4 Integration ................................ ................................ ................................ ................... 11 
4.1 Scope of Delivery ................................ ................................ ............................. 11 
4.1.1 Static Files ................................ ................................ ....................... 11 
4.1.2 Dynamic Files ................................ ................................ .................. 11 
4.2 Include Structure ................................ ................................ .............................. 11 
5 API Description ................................ ................................ ................................ ........... 12 
5.1 Type Definitions ................................ ................................ ............................... 12 
5.2 Interrupt Service Routines provided by CRC ................................ .................... 12 
5.3 Services provided by CRC ................................ ................................ ............... 12 
5.3.1 Crc_CalculateCRC8 ................................ ................................ ......... 12 
5.3.2 Crc_CalculateCRC8H2F ................................ ................................ .. 13 
5.3.3 […]

## Related module

See [Crc](../) for purpose, API, files and dependencies.
