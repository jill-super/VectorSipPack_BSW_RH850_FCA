---
title: "Converted: CanTp"
sidebar:
  order: 2
---

# Converted: Technical Reference — CanTp

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_CanTp.pdf` — 58 pages · original title `MICROSAR CAN Transport Layer`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **CanTp**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR CAN Transport Layer
- Technical Reference
- Status Released
- Technical Reference MICROSAR CAN Transport Layer
- Document Information
- History
- Author Date Version Remarks
- Reference Documents
- Caution
- Contents
- 3.1.2.1 Split CanTp_MainFunction ................................ ............. 14
- 3.1.2.2 Notification of Failed Buffer Request ..............................  14
- 3.1.2.3 Handling of FC Frames with a Reserved STmin ............ 14
- 3.1.2.4 Dynamic and Static BlockSize and STmin ..................... 15

## Key content (extracted text sample)

MICROSAR CAN Transport Layer 
Technical Reference 
 
 
Version 3.01.00 
 
 
 
 
 
 
 
 
 
 
 
Authors Thomas Dedler, Anthony Thomas 
Status Released 
 
 
 
 
 
 
Technical Reference MICROSAR CAN Transport Layer 
© 2017 Vector Informatik GmbH Version 3.01.00 2 
based on template version 5.7.1 
Document Information 
History 
Author Date Version Remarks 
Thomas Dedler 2012-07-11 1.00.00 Initial version 
Thomas Dedler 2012-11-26 1.01.00 Synchronous transmission feature removed 
Thomas Dedler 2013-04-15 1.02.00 > Configuration Hint chapter added 
> Description of Post-Build Loadable 
Thomas Dedler 2013-08-26 1.03.00 > Limitations of Single Channel Optimization 
added 
> Limitation of data length parameter added 
> Dcm OnRequestDetection feature removed 
Thomas Dedler 2014-04-10 1.04.00 > Synchronous / Asynchronous Transmission 
> AR4.1.2 PduR API support 
Thomas Dedler 2014-08-22 2.00.00 > SingleChannel optimization removed 
> Support of CAN-FD added 
> Application callbacks changed 
> Postbuild-Build Selectable 
Thomas Dedler 2015-01-12 2.01.00 > Missing description of CanTp_InitMemory() 
added 
> Reentrancy of CanTp_GetVersionInfo() 
corrected 
> Minor clarifications in regarding CAN-FD 
Thomas Dedler 2015-07-01 2.02.00 > Separation Time by Application 
> Dynamic BS feature description adapted 
according to latest ISO specification 
Thomas Dedler 2015-12-11 3.00.00 > Obsolete features removed: 
> Notification of Failed Cancellations 
> Ignore FC with invalid flow status 
> Ignore FC with reserved STmin 
> Ignore CF with wrong sequence number 
> Clarification of performance parameter 
configuration 
> Rework of Critical Section chapter 
> Hint for DET configuration added 
Anthony Thomas 2016-08-05 3.00.01 > Updated document template 
> Documented features, deviations and 
extensions properly. 
Anthony Thomas 2017-03-24 3.01.00 > Mixed11 address extension forwarding 
 
Technical Reference MICROSAR CAN Transport Layer 
© 2017 Vector Informatik GmbH Version 3.01.00 3 
based on template version 5.7.1 
Reference Documents 
No. Source Title Version 
[1] AUTOSAR AUTOSAR_SWS_CANTransportLayer.pdf 4.0.0 
[2] AUTOSAR AUTOSAR_SWS_CANInterface.pdf 5.0.0 
[3] AUTOSAR AUTOSAR_SWS_PDURouter.pdf 3.2.0 
[4] ISO /ISO/TF2/: ISO FDIS 15765-2; Road vehicles — 
Diagnostics on CAN — Part 2: Network layer services 
2015 
[5] AUTOSAR AUTOSAR_SWS_DevelopmentErrorTracer.pdf 3.2.0 
[6] Vector TechnicalReference_Asr_Dbg.pdf 1.0.0 
[7] Vector TechnicalReference_PostBuildLoadable.pdf 1.2.0 
[8] Vector TechnicalReference_IdentityManager.pdf 1.0.0 
[9] Vector TechnicalReference_Det.pdf 2.0.4 
 
 
Technical Reference MICROSAR CAN Transport Layer 
© 2017 Vector Informatik GmbH Version 3.01.00 4 
based on template version 5.7.1 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 
 
 
Caution 
This symbol calls your attention to warnings. 
 
 

Technical Reference MICROSAR CAN Transport Layer 
© 2017 Vector Informatik GmbH Version 3.01.00 5 
based on template version 5.7.1 
Contents 
1 Component History ................................ ................................ ................................ ...... 9 
2 Introduction................................ ................................ ................................ ................. 10 
2.1 Architecture Overview ................................ ................................ ...................... 11 
3 Functional Description ................................ ................................ ............................... 13 
3.1 Features ................................ ................................ ................................ .......... 13 
3.1.1 Deviations ................................ ................................ ........................ 13 
3.1.2 Additions/ Extensions ................................ ................................ ....... 14 
3.1.2.1 Split CanTp_MainFunction ................................ ............. 14 
3.1.2.2 Notification of Failed Buffer Request .............................. 14 
3.1.2.3 Handling of FC Frames with a Reserved STmin ............ 14 
3.1.2.4 Dynamic and Static BlockSize and STmin ..................... 15 
3.1.2.5 Dynamic Channel […]

## Related module

See [CanTp](../) for purpose, API, files and dependencies.
