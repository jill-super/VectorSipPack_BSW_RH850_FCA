---
title: "Converted: FblCw"
sidebar:
  order: 2
---

# Converted: Technical Reference — FblCw

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_FblCw.pdf` — 28 pages · original title `Flash Bootloader`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **FblCw**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- Flash Bootloader
- Technical Reference
- Communication Wrapper PDU Router
- Status Released
- Technical Reference Flash Bootloader
- Document Information
- History
- Author Date Version Remarks
- Reference Documents
- Configurator
- Caution
- Contents
- Illustrations
- Tables

## Key content (extracted text sample)

Flash Bootloader 
Technical Reference 
 
Communication Wrapper PDU Router 
Version 3.02.00 
 
 
 
 
 
 
 
 
 
 
Authors Jörn Herwig, Ralf Hägenläuer, Andreas Wenckebach, 
Achim Strobelt, Gunnar Meiss 
Status Released 
 
 
 
 
 
Technical Reference Flash Bootloader 
© 2018 Vector Informatik GmbH Version 3.02.00 2 
based on template version 6.0.1 
Document Information 
History 
 
Author Date Version Remarks 
Achim Strobelt 2017-12-20 3.00.00 Cfg5 configuration module 
Achim Strobelt 2018-03-12 3.01.00 Decline requests, ComM handling 
Achim Strobelt 2018-05-05 3.02.00 Remove usage of ASR ComM module for CAN 
 
Reference Documents 
No. Source Title Version 
[1] Vector User Manual Flash Bootloader 2.7 
[2] Vector Technical Reference MICROSAR PDU Router – DaVinci 
Configurator 
3.00.00 
 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 
 

Technical Reference Flash Bootloader 
© 2018 Vector Informatik GmbH Version 3.02.00 3 
based on template version 6.0.1 
Contents 
1 Introduction ................................ ................................ ................................ .................... 6 
1.1 Architecture Overview ................................ ................................ .............................. 6 
2 Functional Description ................................ ................................ ................................ .. 7 
2.1 Features ................................ ................................ ................................ ................... 7 
2.1.1 Multiple Bus Types ................................ ................................ .......................... 7 
2.1.2 Multiple Connections ................................ ................................ ....................... 7 
2.1.3 Baud Rate Switch ................................ ................................ ............................ 8 
3 Integration ................................ ................................ ................................ ...................... 9 
3.1 Scope of Delivery ................................ ................................ ................................ ..... 9 
3.1.1 Static Files ................................ ................................ ................................ ...... 9 
3.1.2 Generated Files ................................ ................................ ............................... 9 
4 Configuration................................ ................................ ................................ ................ 11 
4.1 Preparation ................................ ................................ ................................ ............ 11 
4.2 DaVinci Configurator ................................ ................................ .............................. 11 
4.2.1 Project Creation ................................ ................................ ............................ 12 
4.2.1.1 Load Network Description File ................................ ................................ 12 
4.2.1.2 Component Selection ................................ ................................ ............. 13 
4.2.2 DCM Module Configuration ................................ ................................ ........... 15 
4.2.2.1 DcmDsl Section ................................ ................................ ...................... 16 
4.2.2.2 DcmGeneral Section ................................ ................................ .............. 17 
4.2.2.3 DcmDslConnections ................................ ................................ ............... 18 
4.2.3 FlexRay Interface Module Configuration ................................ ....................... 19 
4.3 Manual Configurations ................................ ................................ ........................... 19 
4.3.1 ComM Channel Configuration ................................ ................................ ....... 19 
4.4 Compiler and Linker Settings ................................ ................................ ................. 19 
5 Interaction with Application Software ................................ ................................ ......... 21 
5.1 Address Configuration […]

## Related module

See [FblCw](../) for purpose, API, files and dependencies.
