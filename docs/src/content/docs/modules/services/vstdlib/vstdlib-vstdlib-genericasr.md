---
title: "Converted: VStdLib"
sidebar:
  order: 2
---

# Converted: Technical Reference — VStdLib

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_VStdLib_GenericAsr.pdf` — 26 pages · original title `MICROSAR VStdLib`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **VStdLib**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR VStdLib
- Technical Reference
- Generic implementation of the Vector Standard Library
- Authors Torsten Kercher
- Status Released
- Technical Reference MICROSAR VStdLib
- Document Information
- History
- Author Date Version Remarks
- Reference Documents
- Caution
- Contents
- Illustrations
- Tables

## Key content (extracted text sample)

MICROSAR VStdLib 
Technical Reference 
 
Generic implementation of the Vector Standard Library 
Version 1.00.01 
 
 
 
 
 
 
 
 
 
 
 
Authors Torsten Kercher 
Status Released 
 
 
 
 
 
 
Technical Reference MICROSAR VStdLib 
© 2016 Vector Informatik GmbH Version 1.00.01 2 
based on template version 5.9.0 
Document Information 
 
History 
Author Date Version Remarks 
Torsten Kercher 2015-05-04 1.00.00 Creation 
Torsten Kercher 2016-04-12 1.00.01 Update to new CI, no changes in content 
 
 
Reference Documents 
No. Source Title Version 
[1] AUTOSAR AUTOSAR_TR_BSWModuleList.pdf 1.6.0 
[2] AUTOSAR AUTOSAR_SWS_DevelopmentErrorTracer.pdf 3.2.0 
 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 

Technical Reference MICROSAR VStdLib 
© 2016 Vector Informatik GmbH Version 1.00.01 3 
based on template version 5.9.0 
Contents 
1 Component History ................................ ................................ ................................ ...... 5 
2 Introduction................................ ................................ ................................ ................... 6 
2.1 Architecture Overview ................................ ................................ ........................ 6 
3 Functional Description ................................ ................................ ................................ . 8 
3.1 Features ................................ ................................ ................................ ............ 8 
3.2 Initialization and Main Functions ................................ ................................ ........ 8 
3.3 Error Handling ................................ ................................ ................................ .... 8 
4 Integration ................................ ................................ ................................ ..................... 9 
4.1 Scope of Delivery ................................ ................................ ............................... 9 
4.2 Include Structure ................................ ................................ ................................ 9 
4.3 Critical Sections ................................ ................................ ................................ . 9 
4.4 Compiler Abstraction and Memory Mapping ................................ ..................... 10 
4.5 Integration Hints ................................ ................................ ............................... 11 
5 API Description ................................ ................................ ................................ ........... 12 
5.1 Type Definitions ................................ ................................ ............................... 12 
5.2 Services provided by VStdLib ................................ ................................ .......... 12 
5.3 Services used by VStdLib ................................ ................................ ................ 22 
6 Configuration ................................ ................................ ................................ .............. 23 
6.1 Configuration Variants ................................ ................................ ...................... 23 
6.2 Manual Configuration in Header File ................................ ................................ 23 
7 Abbreviations ................................ ................................ ................................ .............. 25 
8 Contact ................................ ................................ ................................ ........................ 26 
 
 
 
Technical Reference MICROSAR VStdLib 
© 2016 Vector Informatik GmbH Version 1.00.01 4 
based on template version 5.9.0 
Illustrations 
Figure 2-1 AUTOSAR 4.x Architecture Overview ................................ ......................... 6 
Figure 2-2 Interfaces to adjacent modules ................................ ................................ ... 7 
Figure 4-1 Include Structure ................................ ................................ ........................ 9 
 
 
Tables 
Table 1-1 Component history................................ ................................ […]

## Related module

See [VStdLib](../) for purpose, API, files and dependencies.
