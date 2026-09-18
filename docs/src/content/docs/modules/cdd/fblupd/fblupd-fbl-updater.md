---
title: "Converted: FBL Updater"
sidebar:
  order: 2
---

# Converted: Technical Reference — FBL Updater

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_FBL_Updater.pdf` — 24 pages · original title `Flash Bootloader Updater`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **FBL Updater**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- Flash Bootloader Updater
- Technical Reference
- Updating the Flash Bootloader to a new version
- Status Released
- Technical Reference Flash Bootloader Updater
- Document Information
- History
- Author Date Version Remarks
- Marco Riedl
- Preparing new FBL version
- Contents
- Illustrations
- Tables
- 1 Introduction

## Key content (extracted text sample)

Flash Bootloader Updater 
Technical Reference 
 
Updating the Flash Bootloader to a new version 
Version 1.02.00 
 
 
 
 
 
 
 
 
 
 
Authors Torben Stößel, Jörn Herwig, Marco Riedl, Robert 
Schäffner 
Status Released 
 
 
 
 
 
Technical Reference Flash Bootloader Updater 
© 2018 Vector Informatik GmbH Version 1.02.00 2 
based on template version 6.0.1 
Document Information 
History 
Author Date Version Remarks 
Torben Stößel 
Jörn Herwig 
Marco Riedl 
2016-10-20 1.00.00 Initial version 
Marco Riedl 
Robert Schäffner 
2018-02-01 1.01.00 Fixed typos Rephrase 
sentence in chapter “2.2.3.1 
Hardware support” for RL78 
Added chapter “4 Testing the 
Updater” 
Marco Riedl 2018-06-29 1.02.00 Reworked chapter 3.2 
Preparing new FBL version 
 
Technical Reference Flash Bootloader Updater 
© 2018 Vector Informatik GmbH Version 1.02.00 3 
based on template version 6.0.1 
Contents 
1 Introduction ................................ ................................ ................................ .................... 6 
1.1 Overview ................................ ................................ ................................ .................. 6 
2 Update process ................................ ................................ ................................ .............. 7 
2.1 Download of Updater ................................ ................................ ................................ 7 
2.2 Update process ................................ ................................ ................................ ........ 8 
2.2.1 Initialization of communication stack ................................ ............................... 8 
2.2.2 Initialization of the Flash Driver ................................ ................................ ....... 8 
2.2.3 Preparing reset safe FBL Updater ................................ ................................ ... 8 
2.2.3.1 Hardware support ................................ ................................ ..................... 9 
2.2.3.2 Bootmanager ................................ ................................ ............................ 9 
2.2.4 Erasure of FBL Memory Area ................................ ................................ .......... 9 
2.2.5 Programming of new FBL version ................................ ................................ ... 9 
2.2.6 Verification of new FBL ................................ ................................ .................... 9 
2.2.7 Validation of new FBL ................................ ................................ .................... 10 
2.2.8 Invalidation of Updater ................................ ................................ .................. 10 
2.2.9 Erasure of the FBL Updater ................................ ................................ ........... 10 
2.2.10 Reset ................................ ................................ ................................ ............ 10 
2.3 Reprogramming the Application................................ ................................ .............. 10 
3 Integration ................................ ................................ ................................ .................... 11 
3.1 Scope of Delivery ................................ ................................ ................................ ... 11 
3.1.1 Core Files ................................ ................................ ................................ ...... 11 
3.1.2 Application files ................................ ................................ ............................. 11 
3.1.2.1 OEM specific application files ................................ ................................ . 11 
3.1.2.2 Hardware specific application files ................................ .......................... 12 
3.1.3 Script files ................................ ................................ ................................ ..... 12 
3.2 Preparing new FBL version ................................ ................................ .................... 12 
3.3 Flash Driver ................................ ................................ ................................ ............ 13 
3.4 Updater configuration ................................ ................................ ............................. 14 
4 Testing the Updater ................................ ................................ ................................ ...... 15 
5 API Description ................................ […]

## Related module

See [FblUpd](../) for purpose, API, files and dependencies.
