---
title: "Converted: Det"
sidebar:
  order: 2
---

# Converted: Technical Reference — Det

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_Det.pdf` — 32 pages · original title `MICROSAR [BSW module]`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **Det**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR DET
- Technical Reference
- Status Released
- Technical Reference MICROSAR DET
- Document Information
- History
- Author Date Version Remarks
- Configurator 5
- BCD-coded return value of
- Reference Documents
- Scope of the Document
- Caution
- Contents
- 3.6.1.4 Filtering of DLT forwarding ................................ ............. 16

## Key content (extracted text sample)

MICROSAR DET 
Technical Reference 
 
 
Version 10.0.0 
 
 
 
 
 
 
 
 
 
 
 
Authors Hartmut Hörner 
Status Released 
 
 
 
 
 
Technical Reference MICROSAR DET 
© 2017 Vector Informatik GmbH Version 10.0.0 2 
based on template version 6.0.1 
Document Information 
History 
Author Date Version Remarks 
Hartmut Hörner 2007-11-29 1.0 Initial version 
Hartmut Hörner 2008-01-03 1.1 Update to AUTOSAR 3 
Hartmut Hörner 2008-04-14 1.2 Naming changed to AUTOSAR short 
name, screen shots updated. 
(ESCAN00025687) 
Hartmut Hörner 2008-09-16 1.3 Added DET extension mechanism based 
on callout. 
Added chapter 4.4. 
Hartmut Hörner 2010-01-13 2.0 Update to AUTOSAR 4 
Hartmut Hörner 2012-04-20 2.1 Added usage hints related to silent BSW 
concept in 4.7. 
(ESCAN00058419) 
Hartmut Hörner 2013-04-09 2.2 Added Configurator 5 and service port 
interface 
(ESCAN00066511) 
Hartmut Hörner 2013-09-13 2.3 Added DLT forwarding support for 
Configurator 5 
(ESCAN00068394, ESCAN00069807) 
Hartmut Hörner 2014-12-10 2.3.1 Added description of 
BCD-coded return value of 
Det_GetVersionInfo() 
(ESCAN00079310) 
Hartmut Hörner 2015-06-12 2.4.0 File name changed 
(ESCAN00081049) 
Added chapter 4.2. 
Hartmut Hörner 2016-12-24 10.0.0 Update to AUTOSAR 4.3 (FEAT-1939) 
Reference Documents 
No. Source Title Version 
[1] AUTOSAR AUTOSAR_SWS_DET.pdf 4.3.0 
[2] AUTOSAR AUTOSAR_BasicSoftwareModules.pdf V1.0.0 
 
 
Technical Reference MICROSAR DET 
© 2017 Vector Informatik GmbH Version 10.0.0 3 
based on template version 6.0.1 
Scope of the Document 
This technical reference describes the general use of the MICROSAR Default Error Tracer 
(DET). 
Note that this release of the DET supports only AUTOSAR 4 and the configuration tool 
Configurator 5. If you need a DET module for previous AUTOSAR versions or tools an 
older version is required. 
 
 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 

Technical Reference MICROSAR DET 
© 2017 Vector Informatik GmbH Version 10.0.0 4 
based on template version 6.0.1 
Contents 
1 Component History ................................ ................................ ................................ ...... 7 
2 Introduction................................ ................................ ................................ ................... 8 
2.1 Architecture Overview ................................ ................................ ........................ 8 
3 Functional Description ................................ ................................ ............................... 10 
3.1 Features ................................ ................................ ................................ .......... 10 
3.1.1 Deviations ................................ ................................ ........................ 10 
3.1.2 Additions/ Extensions ................................ ................................ ....... 10 
3.1.3 Limitations ................................ ................................ ........................ 11 
3.2 Initialization ................................ ................................ ................................ ...... 11 
3.3 States ................................ ................................ ................................ .............. 11 
3.4 Main Functions ................................ ................................ ................................ 11 
3.5 Error Handling ................................ ................................ ................................ .. 11 
3.5.1 Development Error Reporting ................................ ........................... 11 
3.5.2 Production Code Error Reporting ................................ ..................... 12 
3.6 Handling of development errors - Debugging with the DET .............................. 12 
3.6.1 Extended Debug Features ................................ ............................... 12 
3.6.1.1 Filters ................................ ................................ ............. 13 
3.6.1.2 Logging ................................ ................................ .......... 14 
3.6.1.3 Break handler ................................ ................................ 15 
3.6.1.4 Filtering of […]

## Related module

See [Det](../) for purpose, API, files and dependencies.
