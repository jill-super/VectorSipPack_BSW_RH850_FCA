---
title: "Converted: Can (RH850 MCAN driver)"
sidebar:
  order: 2
---

# Converted: Technical Reference — Can (RH850 MCAN driver)

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_Can_RH850_MCAN.pdf` — 102 pages · original title `MICROSAR CAN Driver`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **Can (RH850 MCAN driver)**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR CAN Driver
- Technical Reference
- Renesas RH850/P1x-C  MCAN
- Status Released
- Technical Reference    MICROSAR CAN Driver
- 1 Document Information
- 1.1 History
- Author Date Version Remarks
- Added MCAN independent Errata for Aurix Plus
- Enhanced description in chapter
- Table 1-1  Document History
- 1.2 Reference Documents
- Table 1-2  Reference Documents
- 1.3 Scope of the Document

## Key content (extracted text sample)

MICROSAR CAN Driver 
Technical Reference 
 
Renesas RH850/P1x-C MCAN 
Version 3.00.01 
 
 
 
 
 
 
 
 
 
 
 
 
Authors P . Herrmann 
Status Released 
 
 
 
 
 
Technical Reference MICROSAR CAN Driver 
© 2018 Vector Informatik GmbH Version 3.00.01 2 
1 Document Information 
1.1 History 
Author Date Version Remarks 
P . Herrmann 2017-02-22 1.00.00 Creation based on SPC58xx description 
P . Herrmann 
G.Pflügel 
2017-04-25 1.01.00 Added latest MCAN Bosch Errata (#16, #17, #18) 
Added MCAN independent Errata for Aurix Plus 
G.Pflügel 2017-07-26 2.00.00 Restructure of history 
P . Herrmann 2017-08-03 2.01.00 Updated SPC574Kxx derivative decription for new 
cut 2.4 hardware revision. 
Enhanced description in chapter 
- 4.8.3 “Hardware Loop Check / Timeout 
Monitoring” 
- 4.10 “Hardware Specific” 
G.Pflügel 2017-08-21 2.02.00 - Platform SAM V71 and Traveo merged together 
and renamed to platform Arm32Mcan 
- Platform Telemaco and compiler ARM added to 
platform Arm32Mcan 
P . Herrmann 2017-09-18 2.03.00 Enhanced ch. 4.8.1 “Dev. Error Reporting” 
P . Herrmann 2017-10-05 2.04.00 Added Silent Mode 
P . Herrmann 2017-11-21 2.05.00 Template update, enhanced Silent Mode 
description 
P . Herrmann 2018-01-15 2.06.00 Dynamic MCAN Revision detection 
M. Huse 2018-02-27 2.07.00 Extended Ram Check 
P . Herrmann 2018-03-02 2.08.00 Telemaco3P STA1385 Cut2.1 
G.Pflügel 2018-03-28 2.09.00 Tricore TC38x and TC39x Step_B added 
M. Huse 2018-04-04 2.10.00 BCM89103 added 
M. Huse 2018-04-11 2.11.00 Updated API description 
C. Huo 2018-04-12 2.12.00 TDA3x added 
M. Huse 2018-04-19 3.00.00 Updated document for multi driver compatibility 
M. Huse 2018-05-07 3.00.01 Updated ISR section for multi driver compatibility. 
Table 1-1 Document History 
1.2 Reference Documents 
No. Title Version 
[1] AUTOSAR_SWS_CAN_DRIVER.pdf 2.4.6 + 
3.0.0 + 
4.0.0 
[2] AUTOSAR_BasicSoftwareModules.pdf V1.0.0 
[3] AUTOSAR_SWS BSW Scheduler V1.1.0 
Technical Reference MICROSAR CAN Driver 
© 2018 Vector Informatik GmbH Version 3.00.01 3 
[4] AUTOSAR_SWS_CAN_Interface.pdf 3.2.7 + 
4.0.0 + 
5.0.0 
[5] AN-ISC-8-1118 MICROSAR BSW Compatibility Check V1.0.0 
[6] M_CAN Controller Area Network Errata Sheet REL2015 0701 
[7] Appl. Note AN-ISC-8-1190 CAN Self Diag 1.1.0 
Table 1-2 Reference Documents 
1.3 Scope of the Document 
This document describes the functionality, API and configuration of the MICROSAR CAN 
Driver as specified in [1]. The CAN Driver is a hardware abstraction layer with a 
standardized interface to the CAN Interface layer. 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector’s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 

Technical Reference MICROSAR CAN Driver 
© 2018 Vector Informatik GmbH Version 3.00.01 4 
Content 
1 Document Information ................................ ................................ ................................ . 2 
1.1 History ................................ ................................ ................................ ............... 2 
1.2 Reference Documents ................................ ................................ ....................... 2 
1.3 Scope of the Document................................ ................................ ...................... 3 
2 Hardware Overview ................................ ................................ ................................ .... 10 
3 Introduction................................ ................................ ................................ ................. 11 
3.1 Architecture Overview ................................ ................................ ...................... 11 
4 Functional Description ................................ ................................ ............................... 14 
4.1 Features ................................ ................................ ................................ .......... 14 
4.2 Initialization ................................ ................................ ................................ ...... 19 
4.3 Communication ................................ ................................ ................................ 19 
4.3.1 Mailbox Layout ................................ ................................ ................. 20 
4.3.2 Mailbox Processing […]

## Related module

See [Can](../) for purpose, API, files and dependencies.
