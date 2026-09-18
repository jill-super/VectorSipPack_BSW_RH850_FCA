---
title: "Converted: MemIf"
sidebar:
  order: 2
---

# Converted: Technical Reference — MemIf

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_MemIf.pdf` — 25 pages · original title `YourTopic`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **MemIf**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR MemIf
- Technical Reference
- Status Released
- Technical Reference MICROSAR MemIf
- 1 Document Information
- 1.1 History
- Author Date Version Remarks
- Table 1-1  History of the document
- 1.2 Reference Documents
- Table 1-2  Reference documents
- 1.3 Scope of the Document
- Please note
- Contents
- 3.4.1.1 Parameter Checking ................................ ........................ 9

## Key content (extracted text sample)

MICROSAR MemIf 
Technical Reference 
 
 
Version 2.02.00 
 
 
 
 
 
 
 
 
 
 
 
Authors Tobias Schmid, Manfred Duschinger, Michael Goß 
Status Released 
 
 
 
 
 
Technical Reference MICROSAR MemIf 
2015, Vector Informatik GmbH Version: 2.02.00 
based on template version 3.1 
2 / 25 
1 Document Information 
1.1 History 
Author Date Version Remarks 
Tobias Schmid 2008-04-14 1.0 Creation of document 
Manfred Duschinger 2013-02-20 1.01.00 Ch. 4.1. Update files 
according to new generator 
Ch. 6 Update Configuration 
Michael Goß 2014-11-21 2.01.01 Typos were corrected and 
content was modified a little 
Michael Goß 2015-04-23 2.02.00 Content was updated 
regarding SafeBSW MemIf 
Table 1-1 History of the document 
1.2 Reference Documents 
No. Title Version 
[1] AUTOSAR_SWS_Mem_AbstractionInterface.pdf V1.4.0 
[2] AUTOSAR_SWS_DET.pdf V2.2.0 
[3] AUTOSAR_BasicSoftwareModules.pdf V1.0.0 
[4] AUTOSAR_SWS_EEPROM_Abstraction.pdf V2.0.0 
[5] AUTOSAR_SWS_Flash_EEPROM_Emulation.pdf V2.0.0 
Table 1-2 Reference documents 
 
1.3 Scope of the Document 
This technical reference describes the general use of module MemIf (AUTOSAR Memory 
Abstraction Interface). 
 
 
Please note 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 

Technical Reference MICROSAR MemIf 
2015, Vector Informatik GmbH Version: 2.02.00 
based on template version 3.1 
3 / 25 
Contents 
1 Document Information ................................ ................................ ................................ . 2 
1.1 History ................................ ................................ ................................ ............... 2 
1.2 Reference Documents ................................ ................................ ....................... 2 
1.3 Scope of the Document................................ ................................ ...................... 2 
2 Introduction................................ ................................ ................................ ................... 6 
2.1 Architecture Overview ................................ ................................ ........................ 7 
3 Functional Description ................................ ................................ ................................ . 8 
3.1 Features ................................ ................................ ................................ ............ 8 
3.2 Initialization ................................ ................................ ................................ ........ 8 
3.3 Main Functions ................................ ................................ ................................ .. 8 
3.4 Error Handling ................................ ................................ ................................ .... 8 
3.4.1 Development Error Reporting ................................ ............................. 8 
3.4.1.1 Parameter Checking ................................ ........................ 9 
4 Integration ................................ ................................ ................................ ................... 11 
4.1 Scope of Delivery ................................ ................................ ............................. 11 
4.1.1 Static Files ................................ ................................ ....................... 11 
4.1.2 Dynamic Files ................................ ................................ .................. 11 
4.2 Include Structure ................................ ................................ .............................. 12 
4.3 Compiler Abstraction and Memory Mapping ................................ ..................... 12 
5 API Description ................................ ................................ ................................ ........... 14 
5.1 Interfaces Overview ................................ ................................ ......................... 14 
5.2 Type Definitions ................................ ................................ ............................... 14 
5.3 Services provided by MemIf ................................ ................................ ............. 15 
5.3.1 MemIf_GetVersionInfo ................................ […]

## Related module

See [MemIf](../) for purpose, API, files and dependencies.
