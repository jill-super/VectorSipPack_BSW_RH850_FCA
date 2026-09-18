---
title: "Converted: FBL Updater RH850"
sidebar:
  order: 2
---

# Converted: Technical Reference — FBL Updater RH850

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_FBL_Updater_RH850.pdf` — 8 pages · original title `FBL Updater RH850`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **FBL Updater RH850**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- FBL Updater RH850
- Technical Reference
- Hardware specific information
- Authors Sebastian Loos
- Status Released
- Technical Reference FBL Updater RH850
- Document Information
- History
- Author Date Version Remarks
- Reference Documents
- Caution
- Contents
- Illustrations
- 1 Introduction

## Key content (extracted text sample)

FBL Updater RH850 
Technical Reference 
 
Hardware specific information 
Version 1.0 
 
 
 
 
 
 
 
 
 
 
Authors Sebastian Loos 
Status Released 
 
 
 
 
 
Technical Reference FBL Updater RH850 
© 2018 Vector Informatik GmbH Version 1.0 2 
based on template version 6.0.1 
Document Information 
History 
Author Date Version Remarks 
Sebastian Loos 2018-06-26 1.00.00 Initial Version 
Reference Documents 
No. Source Title Version 
[1] Vector TechnicalReference_FBL_Updater.pdf 1.xx.xx 
 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 

Technical Reference FBL Updater RH850 
© 2018 Vector Informatik GmbH Version 1.0 3 
based on template version 6.0.1 
Contents 
1 Introduction ................................ ................................ ................................ .................... 5 
1.1 Theory of operation ................................ ................................ ................................ .. 5 
2 Integration ................................ ................................ ................................ ...................... 6 
2.1 Flash Driver Settings ................................ ................................ ................................ 6 
2.2 New Bootloader ................................ ................................ ................................ ........ 6 
3 Configuration................................ ................................ ................................ .................. 7 
4 Contact................................ ................................ ................................ ............................ 8 
 
Technical Reference FBL Updater RH850 
© 2018 Vector Informatik GmbH Version 1.0 4 
based on template version 6.0.1 
Illustrations 
Figure 1-1 Typical configuration for reset-safe Updater ................................ ................ 5 
 
Technical Reference FBL Updater RH850 
© 2018 Vector Informatik GmbH Version 1.0 5 
based on template version 6.0.1 
1 Introduction 
This document will give a brief overview on the Renesas RH850 specific aspects of the FBL 
Updater. A general description of the updater can be found in [1]. 
1.1 Theory of operation 
To ensure a reset-safe update process, the Set-Reset-Vector ability of the FlashLib (FCL) is 
used. 
 
Figure 1-1 Typical configuration for reset-safe Updater 
Prior to erasing the (old) FBL, the Updater will set the reset vector to its own starting address 
as shown in Figure 1-1. If the whole update process is successful finished, it will set the 
reset vector back to the FBL. 
This will avoid that if the update process gets interrupted by e.g. a power -down reset a 
partially deleted or partially written bootloader gets executed. 
1
16K Block 0
16K Block 1
16K Block 2
16K Block 3
32K Block 4
32K Block 5
32K Block 6
32K Block 7
0x00000
RH850 Resetvector
FBL
Updater
Interrupt Vector Table
__usr_init()
0x18000
0x18200
New FBL
Technical Reference FBL Updater RH850 
© 2018 Vector Informatik GmbH Version 1.0 6 
based on template version 6.0.1 
2 Integration 
2.1 Flash Driver Settings 
The RH850 Updater uses the Set-Reset-Vector-Api, which means it requires a Flash Driver 
which is compiled with 
#define FLASH_ENABLE_SET_RESETVECTOR_API 
2.2 New Bootloader 
It may be required that the image of the new FBL is aligned according to the flash segment 
size (0x100). To ensure this, a batch file is provided (FblUpd_Pr epare_Hw.bat). It will be 
used by the other provided preparing batch scripts. 
Technical Reference FBL Updater RH850 
© 2018 Vector Informatik GmbH Version 1.0 7 
based on template version 6.0.1 
3 Configuration 
 
 
Caution 
Add all necessary initializations (especially: Oscillator, PLL settings) to the initialization 
routine ApplFblUpdHwInit(. If the System clock is not set as expected by the 
FlashLib, the Updater will not be able to write the flash memory. 
 
This is especially necessary if the Updater shall be reset-safe, because if it is re-started 
from a reset, the PLL is not initialized. If the Updater is started by the FBL, the FBL has 
already initialized the PLL. 
 
 
The following Reset Vectors need to be configured in the upd_hw_cfg.h: 
> #define […]

## Related module

See [FblUpd](../) for purpose, API, files and dependencies.
