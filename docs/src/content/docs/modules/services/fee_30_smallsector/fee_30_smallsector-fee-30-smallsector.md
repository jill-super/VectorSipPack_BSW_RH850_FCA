---
title: "Converted: Fee_30_SmallSector"
sidebar:
  order: 2
---

# Converted: Technical Reference — Fee_30_SmallSector

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_Fee_30_SmallSector.pdf` — 43 pages · original title `MICROSAR [BSW module]`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **Fee_30_SmallSector**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR Fee
- Technical Reference
- Small Sector
- Status Released
- Technical Reference MICROSAR Fee
- Document Information
- History
- Author Date Version Remarks
- 1.01.00 Chapter ‘Requirements and
- Reference to ProductInformation of
- Reference Documents
- Caution
- Contents
- 3.5.4 Processing of an EraseImmediateBlock Job ................................ .... 15

## Key content (extracted text sample)

MICROSAR Fee 
Technical Reference 
 
Small Sector 
Version 2.0.0 
 
 
 
 
 
 
 
 
 
 
 
Authors Michael Goß, Bernhard Karl 
Status Released 
 
 
 
 
 
Technical Reference MICROSAR Fee 
© 2018 Vector Informatik GmbH Version 2.0.0 2 
based on template version 6.0.1 
Document Information 
History 
Author Date Version Remarks 
virgmi 2016-06-22 1.00.00 Initial version 
virgmi 2016-08-23 
 
2016-09-21 
1.01.00 Chapter ‘Requirements and 
Recommendations’ was added. 
Reference to ProductInformation of 
SmallSectorFee was added. 
virbka 2018-04-04 2.00.00 Chapter ‘Incompatibility between 
SmallSectorFee Version 1.xx.xx and 
2.xx.xx’ was added. 
Chapter ‘Overhead Calculation’ was 
adapted 
New note box in chapter ‘Configuring Flash 
API Services’ 
Chapter ‘Block Configuration’ was 
extended 
Reference Documents 
No. Source Title Version 
[1] AUTOSAR AUTOSAR_SWS_FlashEEPROMEmulation.pdf V2.0.0 
[2] AUTOSAR AUTOSAR_SWS_DevelopmentErrorTracer.pdf V3.2.0 
[3] AUTOSAR AUTOSAR_BasicSoftwareModules.pdf V1.0.0 
[4] Vector ProductInformation_8_MICROSARSmallSectorFee.pdf V1.0.0 
[5] Vector AUTOSAR_SWS_NVRAMManager.pdf V3.2.0 
 
 
 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 

Technical Reference MICROSAR Fee 
© 2018 Vector Informatik GmbH Version 2.0.0 3 
based on template version 6.0.1 
Contents 
1 Component History ................................ ................................ ................................ ...... 6 
2 Introduction................................ ................................ ................................ ................... 7 
2.1 Architecture Overview ................................ ................................ ........................ 8 
3 Functional Description ................................ ................................ ............................... 11 
3.1 Features ................................ ................................ ................................ .......... 11 
3.1.1 Deviations from AUTOSAR R4.0.3 ................................ ................... 11 
3.1.2 Additions/ Extensions ................................ ................................ ....... 12 
3.2 Recommendations ................................ ................................ ........................... 12 
3.3 Initialization ................................ ................................ ................................ ...... 13 
3.4 States ................................ ................................ ................................ .............. 13 
3.4.1 Module States ................................ ................................ .................. 13 
3.4.2 Job States ................................ ................................ ........................ 13 
3.5 Main Functions ................................ ................................ ................................ 14 
3.5.1 Processing of a Read Job ................................ ................................ 14 
3.5.2 Processing of a Write Job ................................ ................................ 14 
3.5.3 Processing of an InvalidateBlock Job ................................ ............... 15 
3.5.4 Processing of an EraseImmediateBlock Job ................................ .... 15 
3.6 Error Handling ................................ ................................ ................................ .. 15 
3.6.1 Development Error Reporting ................................ ........................... 15 
3.6.2 Production Code Error Reporting ................................ ..................... 16 
3.7 Partitions ................................ ................................ ................................ .......... 17 
3.8 Service for handling under-voltage situations ................................ ................... 17 
3.9 MainFunction Triggering ................................ ................................ ................... 18 
4 Integration ................................ ................................ ................................ ................... 19 
4.1 Scope of Delivery ................................ ................................ ............................. 19 […]

## Related module

See [Fee_30_SmallSector](../) for purpose, API, files and dependencies.
