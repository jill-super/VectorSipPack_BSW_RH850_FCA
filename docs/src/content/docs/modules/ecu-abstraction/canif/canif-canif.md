---
title: "Converted: CanIf"
sidebar:
  order: 2
---

# Converted: Technical Reference — CanIf

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_CanIf.pdf` — 71 pages · original title `CAN Interface`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **CanIf**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- CAN Interface
- Technical Reference
- Technical Reference CAN Interface
- 1 Document Information
- 1.1 History
- Author Date Version Remarks
- Eugen Stripling
- ESCAN00066338
- ESCAN00066340
- Adapted according to
- ESCAN00066285
- ESCAN00065289
- ESCAN00066396
- ESCAN00064304

## Key content (extracted text sample)

CAN Interface 
Technical Reference 
 
 
Version 6.11.01 
 
 
 
 
 
 
 
 
 
 
Authors Rüdiger Naas, Eugen Stripling 
Versions: 6.11.01 
Status: Released 
 
 
 
 
 
Technical Reference CAN Interface 
© 2017 Vector Informatik GmbH Version 6.11.01 2 
based on template version 2.10.0 
1 Document Information 
1.1 History 
Author Date Version Remarks 
Eugen Stripling 
Rüdiger Naas 
2012-07-17 5.00 ASR R4.0 Rev 3 
Eugen Stripling 2013-04-03 5.01.00 ESCAN00065368 
ESCAN00066338 
ESCAN00066340 
Adapted according to 
ESCAN00066285 
Adapted according to 
ESCAN00065289 
ESCAN00066396 
Adapted according to 
ESCAN00064304 
Rüdiger Naas 2013-07-24 5.01.01 ESCAN00066794 
Eugen Stripling 2013-09-27 6.00.00 Adapted due to: 
AR4-307: J1939 support 
AR4-438: Dynamic address lookup 
table 
AR4-397: CAN FD support 
Eugen Stripling 2014-05-19 6.01.00 CAN FD support extended: Rx-FD 
and Rx- and Tx-PDUs with up to 
64 bytes payload 
Rüdiger Naas 2014-07-10 6.02.00 Multiple CAN driver support 
Eugen Stripling 2014-08-25 6.02.00 ESCAN00077304, Restriction 
concerning the handling of 
FD/Not-FD FullCAN-Rx-PDUs 
added 
Eugen Stripling 2014-09-22 6.02.00 ESCAN00078524, CanTSyn added, 
Post-build selectable 
Eugen Stripling 2014-11-25 6.03.00 Channel specific J1939 dynamic 
address 
Eugen Stripling 2015-01-26 6.04.00 Chapter 3.8 adapted to changed 
implementation 
Eugen Stripling 2015-05-18 6.05.00 Adapted due to FEAT-366 
Eugen Stripling 2015-11-20 6.06.00 Adapted due to FEAT-1429 
Eugen Stripling 2016-01-09 6.06.00 ESCAN00087340 
Eugen Stripling 2016-02-22 6.07.00 Feature Extended RAM-check 
added, ESCAN00087587 
Eugen Stripling 2016-06-24 6.08.00 Feature: Data checksum added 
Eugen Stripling 2016-09-14 6.09.00 Adapted due to FEAT-2076: 
Technical Reference CAN Interface 
© 2017 Vector Informatik GmbH Version 6.11.01 3 
based on template version 2.10.0 
Behavior of Tx-PDU filter extended 
Eugen Stripling 2016-09-26 6.09.00 Adapted due to FEAT-2024: Set 
reception mode 
Eugen Stripling 2017-01-09 6.10.00 Improved due to ESCAN00093454 
Eugen Stripling 2017-02-13 Adapted due to: FEAT-2140: TMC 
Checksum - Release feature FEAT-
1914 
Eugen Stripling 2017-02-28 ESCAN00094196, deviation from 
AUTOSAR documented by 
ESCAN00094121 added 
Eugen Stripling 2017-08-04 6.11.00 ESCAN00096181 
Eugen Stripling 2017-08-30 6.11.01 Typos corrected 
Table 1-1 History of the Document 
1.2 Reference Documents 
No. Title Version 
[1] AUTOSAR_SWS_CANInterface.pdf 
4.2.2 
5.0.0 
6.0.0 
[2] AUTOSAR_SWS_DevelopmentErrorTracer.pdf 3.2.0 
[3] AUTOSAR_SRS_BSWGeneral.pdf 3.2.0 
Table 1-2 References Documents 
 
 
Please note 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector’s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 

Technical Reference CAN Interface 
© 2017 Vector Informatik GmbH Version 6.11.01 4 
based on template version 2.10.0 
Contents 
1 Document Information ................................ ................................ ................................ . 2 
1.1 History ................................ ................................ ................................ ............... 2 
1.2 Reference Documents ................................ ................................ ....................... 3 
2 Introduction................................ ................................ ................................ ................... 9 
2.1 Architecture Overview ................................ ................................ ........................ 9 
3 Functional Description ................................ ................................ ............................... 11 
3.1 Deviations regarding AUTOSAR standard ................................ ........................ 11 
3.2 Feature List ................................ ................................ ................................ ...... 11 
3.3 Initialization ................................ ................................ ................................ ...... 12 
3.4 Transmission................................ ................................ ................................ .... 13 
3.4.1 Dynamic transmission ................................ ................................ ...... 14 
3.4.2 Transmit-buffer ................................ […]

## Related module

See [CanIf](../) for purpose, API, files and dependencies.
