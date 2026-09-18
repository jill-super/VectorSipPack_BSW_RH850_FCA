---
title: "AN-ISC-8-1173 Share FEE Blocks Between Application and Bootloader"
sidebar:
  order: 1
---

# AN-ISC-8-1173 Share FEE Blocks Between Application and Bootloader

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Application%20notes-lightgrey)

> **Source:** `Doc/ApplicationNotes/AN-ISC-8-1173_Share_FEE_Blocks_Between_Application_and_Bootloader.pdf` — 15 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

**Original metadata:** title `Share FEE Blocks Between Application and Bootloader` · author `Vogel, Nils, Andreas Wenckebach`

## What this document covers

Sharing Fee blocks between application and bootloader: partitioning, NvM/Fee configuration and consistency rules.

## Document outline (extracted headings)

- Share FEE Blocks Between Application and Bootloader
- Application Note AN-ISC-8-1173
- Restrictions Customer confidential - Vector decides
- Table of Contents
- 1.0 Overview
- Share FEE blocks between APPL and bootloader
- 2.0 Preconditions on the FEE Layout
- 2.1 MSR Module Precondition
- 2.2 Config Limitations
- 2.2.1 NvM Configuration in the Bootloader
- 2.2.2 Block Limitation
- 2.3 FEE Feature FeeFblConfig
- 2.3.1 Potential Problem with Regular AR Fee
- Figure 4-4 FEE Sector Switch with Regular AR FEE

## Key content (extracted text sample)

Share FEE Blocks Between Application and Bootloader 
Version 1.01.01 
2017-01-11 
Application Note AN-ISC-8-1173 
 
 
 
Author(s) Vogel, Nils, Andreas Wenckebach 
Restrictions Customer confidential - Vector decides 
Abstract This document shows how to share nonvolatile data between application and bootloader using the 
Vector FEE and DaVinci Configurator Pro for AUTOSAR 4 projects. 
 
Table of Contents 
 
 1 
Copyright © 2017 - Vector Informatik GmbH 
Contact Information: www.vector.com or +49-711-80 670-0 
1.0 Overview .......................................................................................................................................................... 1 
2.0 Preconditions on the FEE Layout .................................................................................................................... 2 
2.1 MSR Module Precondition............................................................................................................................. 2 
2.2 Config Limitations .......................................................................................................................................... 2 
2.2.1 NvM Configuration in the Bootloader .......................................................................................................... 2 
2.2.2 Block Limitation ........................................................................................................................................... 3 
2.3 FEE Feature FeeFblConfig ........................................................................................................................... 3 
2.3.1 Potential Problem with Regular AR Fee ..................................................................................................... 4 
2.3.2 Vector FEE Bootloader Configuration......................................................................................................... 4 
3.0 FEE Configuration with the DaVinci Configurator Pro ..................................................................................... 5 
3.1 Step 1 Configure the NvM/FEE on Application Side. .................................................................................... 5 
3.2 Step 2 Transfer the MEM Stack Configuration to the Bootloader ................................................................. 5 
3.3 Step 3 Adapt the Imported Configuration to Your Needs .............................................................................. 7 
3.4 Step 4 Add the Standard Definition of the NvM ............................................................................................ 8 
3.5 Special configuration Aspects in Non DaVinci Configurator Pro Environments ......................................... 10 
3.5.1 Further ASR Component Stubs required .................................................................................................. 10 
3.5.2 Generation of the Fee Config for the Fbl .................................................................................................. 11 
4.0 Usage of Fee Configuration in Flash Bootloader ........................................................................................... 11 
4.1 Modules Required in the Flash Bootloader ................................................................................................. 11 
4.1.1 Asr BSW Modules to Be Added to Flash Bootloader ............................................................................... 11 […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
