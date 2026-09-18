---
title: "Converted: ComStackLib (_Common)"
sidebar:
  order: 2
---

# Converted: Technical Reference — ComStackLib (_Common)

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_ComStackLib.pdf` — 42 pages · original title `MICROSAR ComStackLib`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **ComStackLib (_Common)**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR ComStackLib
- Technical Reference
- ComStackLib based BSW generators
- Authors Gunnar Meiss
- Status Released
- Technical Reference MICROSAR ComStackLib
- Document Information
- History
- Author Date Version Remarks
- ESCAN00089126 Support a justification for PRQA Rule
- Added chapter Freedom from Interference
- PRQA Rule 3325
- Reference Documents
- Scope of the Document

## Key content (extracted text sample)

MICROSAR ComStackLib 
Technical Reference 
 
ComStackLib based BSW generators 
Version 2.02.00 
 
 
 
 
 
 
 
 
 
 
 
Authors Gunnar Meiss 
Status Released 
 
 
 
 
 
Technical Reference MICROSAR ComStackLib 
© 2017 Vector Informatik GmbH Version 2.02.00 2 
based on template version 5.5.0 
Document Information 
History 
Author Date Version Remarks 
Gunnar Meiss 2013-03-25 1.00.00 initial version 
Gunnar Meiss 2013-08-23 1.01.00 ESCAN00068919 Remove 
<MSN>UseSignedDataTypesInIndexArrays 
ESCAN00070017 Remove <MSN>_Resource.xml 
Gunnar Meiss 2014-10-06 2.00.00 ESCAN00078776 AR4-698: Post-Build Selectable 
(Identity Manager) 
Gunnar Meiss 2014-12-19 2.00.01 ESCAN00080380 Minor typing and grammar corrections 
Gunnar Meiss 2016-03-30 2.00.02 ESCAN00089127 Extend MD_CSL_3355_3356 with the 
aspects of the PRQA Rule 3358 and 3359 
ESCAN00089126 Support a justification for PRQA Rule 
310 and PCSymbolicNonDereferenciateablePointers 
Added chapter Freedom from Interference 
Gunnar Meiss 2016-07-19 2.00.03 ESCAN00091055 Extend 
MD_CSL_3355_3356_3358_3359 with the aspects of 
PRQA Rule 3325 
Gunnar Meiss 2017-03-24 2.01.00 STORYC-534: <MSN>MinimizeNumericalDataTypes is 
always enabled 
Gunnar Meiss 2017-12-19 2.02.00 STORYC-3585: Avoid PRQA Rule 3629 "Union contains 
member of floating type" 
Reference Documents 
No. Source Title Version 
[1] Vector Compliance Documentation MISRA-C:2004 / MICROSAR 2.2.0 
Scope of the Document 
This technical reference describes the general use of the ComStackLib based BSW 
generators. 
 
 
 
 
 
 
 
 
 
Technical Reference MICROSAR ComStackLib 
© 2017 Vector Informatik GmbH Version 2.02.00 3 
based on template version 5.5.0 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 

Technical Reference MICROSAR ComStackLib 
© 2017 Vector Informatik GmbH Version 2.02.00 4 
based on template version 5.5.0 
Contents 
1 Component History ................................ ................................ ................................ ...... 6 
2 Introduction................................ ................................ ................................ ................... 7 
2.1 Architecture Overview ................................ ................................ ........................ 8 
3 Functional Description ................................ ................................ ................................ . 9 
3.1 CONFIG-CLASS of Data ................................ ................................ .................. 10 
3.2 CONFIG-CLASS PRE-COMPILE Optimizations ................................ .............. 10 
3.2.1 Optimize Const Data to Defines ................................ ....................... 10 
3.2.2 Optimize Bool Data in Structs ................................ .......................... 11 
3.2.3 Data Deduplication and Reduction ................................ ................... 12 
3.2.3.1 Equal Data ................................ ................................ ..... 13 
3.2.3.2 Unary and Binary Operations ................................ ......... 14 
3.2.4 Data Streaming ................................ ................................ ................ 15 
3.3 CONFIG-CLASS Independent Optimizations ................................ ................... 16 
3.3.1 Sort Struct Elements ................................ ................................ ........ 16 
3.3.2 Optimize Data Types ................................ ................................ ........ 17 
3.4 SELECTABLE Optimizations ................................ ................................ ............ 18 
3.4.1 Merge of VAR and CONST Based Data ................................ ........... 18 
3.5 Freedom from Interference ................................ ................................ .............. 18 
4 Integration ................................ ................................ ................................ ................... 19 
4.1 Dynamic Files ................................ ................................ ................................ .. 19 
4.2 IMPLEMENTATION-CONFIG-VARIANT dependent Data ................................ 21 
4.3 Optimization Levels […]

## Related module

See [_Common](../) for purpose, API, files and dependencies.
