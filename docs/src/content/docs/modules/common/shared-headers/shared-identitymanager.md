---
title: "Converted: Identity Manager"
sidebar:
  order: 2
---

# Converted: Technical Reference — Identity Manager

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_IdentityManager.pdf` — 22 pages · original title `MICROSAR Identity Manager`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **Identity Manager**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR Identity Manager
- Technical Reference
- Post-Build Selectable
- Authors Hannes Haas
- Status Released
- Technical Reference MICROSAR Identity Manager
- Document Information
- History
- Author Date Version Remarks
- Global Root Structure Customization now
- Reference Documents
- Scope of the Document
- Caution
- Contents

## Key content (extracted text sample)

MICROSAR Identity Manager 
Technical Reference 
 
Post-Build Selectable 
Version 1.1.1 
 
 
 
 
 
 
 
 
 
 
 
Authors Hannes Haas 
Status Released 
 
 
 
 
 
Technical Reference MICROSAR Identity Manager 
2015, Vector Informatik GmbH Version: 1.1.1 
based on template version 5.7.1 
2 / 22 
Document Information 
History 
Author Date Version Remarks 
Hannes Haas 2014-10-29 1.0.0 Creation 
Hannes Haas 2015-01-26 1.1.0 ESCAN00080589: global root structure is 
now a structure with one element for each 
variant. 
Global Root Structure Customization now 
possible by configuring the ECUC module. 
Hannes Haas 2015-03-03 1.1.1 Adapted file names of referred 
documentations. 
Reference Documents 
No. Source Title Version 
[1] Vector TechnicalReference_PostBuildLoadable.pdf as delivered 
[2] Vector TechnicalReference_EcuM.pdf as delivered 
[3] Vector TechnicalReference_BswM.pdf as delivered 
Scope of the Document 
This technical reference describes the general aspects of the MICROSAR Identity 
Manager. The document does not describe BSW module specific functionality or 
limitations unless this is essential to understand the overall concept. Module -specific 
details can be found in the documentation of each BSW module. 
This document focuses on BSW functionality. Configuration aspects are described in the 
help system of DaVinci Configurator Pro. 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 

Technical Reference MICROSAR Identity Manager 
2015, Vector Informatik GmbH Version: 1.1.1 
based on template version 5.7.1 
3 / 22 
Contents 
1 Introduction................................ ................................ ................................ ................... 5 
1.1 Comparison to Post-Build Loadable ................................ ................................ ... 6 
2 Functional Description ................................ ................................ ................................ . 7 
2.1 Technical Background ................................ ................................ ........................ 7 
2.2 Features ................................ ................................ ................................ ............ 8 
2.3 Deviations ................................ ................................ ................................ .......... 8 
3 Workflow Overview ................................ ................................ ................................ ....... 9 
3.1 Setting Up a Variant Project ................................ ................................ ............... 9 
3.2 BSW Configuration ................................ ................................ .......................... 11 
3.3 Variance in Application Code ................................ ................................ ............ 11 
3.3.1 Variance of COM Signals ................................ ................................ . 12 
3.3.2 Variance in SWC and BSW APIs ................................ ...................... 12 
3.4 Validation and Code Generation ................................ ................................ ...... 13 
3.5 BSW Initialization ................................ ................................ ............................. 13 
3.5.1 Manual BSW Initialization................................ ................................ . 14 
4 Configuration ................................ ................................ ................................ .............. 15 
4.1 Activating Variance for BSW Modules ................................ .............................. 15 
4.2 Semantics of ECU Configuration Variance ................................ ....................... 16 
5 Integration ................................ ................................ ................................ ................... 18 
5.1 BSW Module Initialization ................................ ................................ ................ 18 
5.1.1 Implementation of EcuM_DeterminePbConfiguration() ..................... 19 
5.1.2 BSWM Module Initialization Auto Configuration ................................ 19 
5.1.3 Global Root Structure Customization ................................ […]

## Related module

See [_Common](../) for purpose, API, files and dependencies.
