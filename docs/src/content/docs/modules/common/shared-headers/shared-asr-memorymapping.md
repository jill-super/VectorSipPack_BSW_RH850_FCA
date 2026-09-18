---
title: "Converted: Memory Mapping (Asr)"
sidebar:
  order: 2
---

# Converted: Technical Reference — Memory Mapping (Asr)

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_Asr_MemoryMapping.pdf` — 20 pages · original title `MICROSAR Memory Mapping`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **Memory Mapping (Asr)**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR Memory Mapping
- Technical Reference
- Authors Eugen Stripling
- Status Released
- Technical Reference MICROSAR Memory Mapping
- Document Information
- History
- Author Date Version Remarks
- ESCAN00095756
- Reference Documents
- Caution
- Contents
- 2.1.1 Declaration of code and data segments in AUTOSAR ........................ 7
- 2.1.2 Mapping of code and data segments to a dedicated memory area ..... 8

## Key content (extracted text sample)

MICROSAR Memory Mapping 
Technical Reference 
 
 
Version 1.3.0 
 
 
 
 
 
 
 
 
 
 
 
Authors Eugen Stripling 
Status Released 
 
 
 
 
 
Technical Reference MICROSAR Memory Mapping 
© 2017 Vector Informatik GmbH Version 1.3.0 2 
based on template version 5.6.0 
Document Information 
History 
Author Date Version Remarks 
Eugen Stripling 2013-04-12 1.00.00 Creation - ESCAN00064655 
Eugen Stripling 2013-05-29 1.00.01 Some typos corrected 
Eugen Stripling 2016-09-27 1.01.00 FEATC-317 / FEAT-2002: 64-bit memory 
section keywords added 
Eugen Stripling 2017-01-16 1.02.00 ESCAN00093572: 2.1.4 chapter added 
Eugen Stripling 2017-07-18 1.03.00 Chapters 2.1 and 2.1.4 adapted due to 
ESCAN00095756 
Reference Documents 
No. Source Title Version 
[1] AUTOSAR AUTOSAR_SWS_MemoryMapping.pdf 1.4.0 
[2] AUTOSAR AUTOSAR_SWS_MemoryMapping.pdf 4.2.2 
[3] AUTOSAR AUTOSAR_SWS_CompilerAbstraction.pdf 3.2.0 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 

Technical Reference MICROSAR Memory Mapping 
© 2017 Vector Informatik GmbH Version 1.3.0 3 
based on template version 5.6.0 
Contents 
1 Introduction................................ ................................ ................................ ................... 5 
2 Functional Description ................................ ................................ ................................ . 6 
2.1 Memory section keywords ................................ ................................ .................. 6 
2.1.1 Declaration of code and data segments in AUTOSAR ........................ 7 
2.1.2 Mapping of code and data segments to a dedicated memory area ..... 8 
2.1.3 Example: Mapping of data to a post-build memory section................. 9 
2.1.4 Usage of AUTOSAR 4.2.2 BSW module ................................ .......... 11 
3 Appendix ................................ ................................ ................................ ..................... 12 
3.1 Sub-keywords used in the memory section and compiler specific keywords .... 12 
3.2 Memory section keywords ................................ ................................ ................ 12 
3.2.1 Memory section keywords for code ................................ .................. 13 
3.2.2 Memory section keywords for constants ................................ ........... 13 
3.2.3 Memory section keywords for variables................................ ............ 14 
3.3 Compiler specific keywords ................................ ................................ .............. 17 
4 Glossary and Abbreviations ................................ ................................ ...................... 19 
4.1 Abbreviations ................................ ................................ ................................ ... 19 
5 Contact ................................ ................................ ................................ ........................ 20 
 
Technical Reference MICROSAR Memory Mapping 
© 2017 Vector Informatik GmbH Version 1.3.0 4 
based on template version 5.6.0 
Illustrations 
Figure 2-1 Files: MemMap.h, MemMap_Common.h and Compiler_Cfg.h ................... 7 
 
Tables 
Table 3-1 Explanation of sub-keywords used in the memory section and compiler 
specific keywords ................................ ................................ ..................... 12 
Table 3-2 Memory sections for code ................................ ................................ ......... 13 
Table 3-3 Memory sections for constants ................................ ................................ . 13 
Table 3-4 Change of memory section keywords for constants in ASR 4.0.3 ............. 14 
Table 3-5 Memory sections for variables ................................ ................................ .. 15 
Table 3-6 Change of memory section keywords for variables in ASR 4.0.3 .............. 17 
Table 3-7 Compiler specific keywords and the related memory sections they used 
for ................................ ................................ ................................ ............. 18 
Table 4-1 Abbreviations ................................ ................................ ............................ 19 
 
 […]

## Related module

See [_Common](../) for purpose, API, files and dependencies.
