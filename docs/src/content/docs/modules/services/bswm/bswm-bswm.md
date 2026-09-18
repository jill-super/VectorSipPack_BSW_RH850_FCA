---
title: "Converted: BswM"
sidebar:
  order: 2
---

# Converted: Technical Reference — BswM

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_BswM.pdf` — 68 pages · original title `Basic Software Mode Manager`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **BswM**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR BswM
- Technical ReferenceTechnical Reference
- Status Released
- Document Information
- History
- Author Date Version Remarks
- Deletion of limitations in
- DET errors added in chapter
- Dynamic files added in
- Figure 3-3
- Partition
- Reference Documents
- Scope of the Document
- Caution

## Key content (extracted text sample)

MICROSAR BswM 
Technical ReferenceTechnical Reference 
 
 
Version 8.01.00 
 
 
 
 
 
 
 
 
 
 
 
Authors Leticia Garcia Herrera, Thomas Kuhl, Philipp Ritter, 
Jochen VorreiterLeticia Garcia Herrera, Thomas Kuhl, 
Philipp Ritter, Jochen Vorreiter 
Status Released 
 
 
 
 
 
Technical ReferenceTechnical Reference Basic Software Mode Manager 
© 2017 Vector Informatik GmbH Version 8.01.00 2 
based on template version 4.11.3 
Document Information 
History 
Author Date Version Remarks 
Leticia Garcia, Thomas Kuhl 2012-08-02 1.00.00 Creation of document. 
Leticia Garcia, Thomas Kuhl 2012-09-27 1.01.00 Addition of feature, support of 
EthSM . Chapters 3.1, 4.1, 
5.2and 6.3. 
Leticia Garcia, Thomas Kuhl 2013-01-31 1.02.00 Addition of feature, support of 
NvM. Chapter 3.1, 4.1, 5.2 
and 5.3. 
Leticia Garcia, Thomas Kuhl 2012-03-26 1.03.00 Support of Post-build variant. 
Chapters 4.1, 4.2, 5.1and 5.2. 
 
Deviation from AUTOSAR. 
Header included: 
Com_Types.h. Chapter 6.1 
Leticia Garcia 2013-10-21 2.00.00 Addition of extension in 
chapter 6.2. 
Deletion of limitations in 
chapter 6.3. 
DET errors added in chapter 
3.6.1. 
Dynamic files added in 
chapter 4.1.2. 
Chapter 4.2 was changed. 
Chapter 4.3 was added. 
Leticia Garcia 2013-12-04 2.00.01 Chapter 3.3 was extended. 
Chapter 3.4.2 was added. 
Chapter 3.6.1 error code 
added. 
Chapter 4.5 was extended 
Chapter 6.2 was extended. 
Leticia Garcia 2013-02-18 2.01.00 Extended chapters: 3.1, 3.1.2, 
3.6.1, 4.1.1, 5.2.15, 5.2.16, 
5.2.33, 5.2.34, 5.2.35, 5.2.36 
5.3 and 6.2.1. 
Added chapters: 4.3.3, 5.6, 
and 6.2.2. Removed deviation 
about 
Com_IpduGroupControl 
usage. 
Philipp Ritter 2014-06-13 3.00.00 Extended chapters: 3.1.2, 3.5, 
5.6.1, 6.2.1, 6.2.8 
Added chapters: 5.2.37, 
6.2.10, 6.2.11 
Updated Figures: Figure 3-2, 
Technical ReferenceTechnical Reference Basic Software Mode Manager 
© 2017 Vector Informatik GmbH Version 8.01.00 3 
based on template version 4.11.3 
Figure 3-3 
Philipp Ritter 2014-10-22 4.00.00 Extended Chapters: 3.1, 
3.6.1, 4.1.1, 4.3.3, 5.2.4 
Added chapters: 5.2.38 
Philipp Ritter 2015-02-02 5.00.00 Extended chapters: 3.6.1, 
4.3.3, 6.3.3, 6.3.4 
Added chapters: 5.2.19 
Removed: Limitation for 
multiple configurations 
Philipp Ritter 2015-07-29 6.00.00 Extended chapters: 3.1, 3.1.2, 
3.6.1, 4.3.3, 5.3 
Added chapters: 4.3.4, 
5.2.23, 5.2.27, 5.2.28, 5.2.29, 
5.2.30, 5.2.31, 5.2.32 
Philipp Ritter 2015-12-10 6.00.01 Updated Figure 4-6 
Jochen Vorreiter 2016-11-15 7.00.00 Added chapters: 5.2.8 and 
5.2.12 
Jochen Vorreiter 2017-09-27 8.00.00 Added support for Multi 
Partition 
Jochen Vorreiter 2017-12-20 8.01.00 Extended chapter 3.6 
Reference Documents 
No. Source Title Version 
[1] AUTOSAR AUTOSAR_SWS_BSWModeManager.pdf 1.4.0 
[2] AUTOSAR AUTOSAR_EXP_ModemanagementGuide 2.1.0 
[3] AUTOSAR AUTOSAR_SWS_DevelopmentErrorTracer.pdf 3.2.0 
[4] AUTOSAR AUTOSAR_TR_BSWModuleList.pdf 1.6.0 
[5] AUTOSAR AUTOSAR_SWS_DiagnosticEventManager.pdf 4.2.0 
[6] Vector TechnicalReference_Rte.pdf see delivery 
[7] Vector TechnicalReference_PostBuildLoadable.pdf see delivery 
[8] Vector TechnicalReference_Com.pdf see delivery 
[9] Vector TechnicalReference_IdentityManager.pdf see delivery 
 
 
 
 
 
 
 
 
Technical ReferenceTechnical Reference Basic Software Mode Manager 
© 2017 Vector Informatik GmbH Version 8.01.00 4 
based on template version 4.11.3 
 
 
Scope of the Document 
This technical reference describes the gener al use of the AUTOSAR Basic Software 
module BSW Mode Manager (BswM). 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector’s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 

Technical ReferenceTechnical Reference Basic Software Mode Manager 
© 2017 Vector Informatik GmbH Version 8.01.00 5 
based on template version 4.11.3 
Contents 
1 Component History ................................ ................................ ................................ .... 10 
2 Introduction................................ ................................ ................................ ................. 11 
2.1 Architecture Overview ................................ ................................ ...................... 11 
3 Functional Description ................................ ................................ […]

## Related module

See [BswM](../) for purpose, API, files and dependencies.
