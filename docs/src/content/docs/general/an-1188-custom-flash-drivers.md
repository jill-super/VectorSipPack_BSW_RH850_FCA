---
title: "AN-ISC-8-1188 Custom Flash Drivers"
sidebar:
  order: 1
---

# AN-ISC-8-1188 Custom Flash Drivers

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Application%20notes-lightgrey)

> **Source:** `Doc/ApplicationNotes/AN-ISC-8-1188_Custom_Flash_Drivers.pdf` — 7 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

**Original metadata:** title `Custom Flash Drivers` · author `Alexander Starke`

## What this document covers

Writing/adapting custom flash drivers (flashdrv API, FblMem interface) for new derivatives.

## Document outline (extracted headings)

- Custom Flash Drivers
- Application Note  AN-ISC -8-1188
- Author Alexander Starke
- Table of Contents
- 1 Overview
- Note
- 2 HIS Flash Driver Interface
- 3 Polling Function
- 3.1 General Information
- Caution
- 3.2 Internal Bootloader Time Base
- 3.3 Watchdog Handling
- Figure 3-1 GENy
- Figure 3-2 DaVinci Configurator

## Key content (extracted text sample)

Custom Flash Drivers 
Version 1.0 
2016- 02- 16 
Application Note AN-ISC -8-1188 
Author Alexander Starke 
Restrictions Customer confidential – Vector decides 
Abstract This application note describes the steps to be taken when embedding a custom flash 
driver into a Vector Bootloader 
 
 
Table of Contents 
1 Overview ........................................................................................................................................ 2 
2 HIS Flash Driver Interface ............................................................................................................ 2 
3 Polling Function ............................................................................................................................ 3 
3.1 General Information ............................................................................................................. 3 
3.2 Internal Bootloader Time Base ............................................................................................ 4 
3.3 Watchdog Handling .............................................................................................................. 4 
3.4 (Adaptive) RCR-RP Handling .............................................................................................. 4 
3.5 Pipelined Programming (Early Acknowledge) ..................................................................... 5 
3.6 Pipelined Verification ........................................................................................................... 5 
4 Downloadable Flash Driver .......................................................................................................... 6 
5 Additional Resources ................................................................................................................... 7 
6 Contacts ......................................................................................................................................... 7 
 
 
Custom Flash Drivers 
Copyright © 2016 - Vector Informatik GmbH 2 
Contact Information: www.vector.com or +49-711-80 670-0 
1 Overview 
The Vector Bootloader uses a standardized flash API, which has been developed by the HIS 
consortium. This standardized flash API offers the possibility to easily extend a Vector Bootloader by 
custom flash drivers. 
Custom flash drivers might be used for various reasons: 
> Adding support for updating additional external flash memory devices 
> Adding support for updating additional external EEPROM devices 
> Adding support for multi-processor flashing 
 
 
Note 
Vector offers implementation services for any of the above options. Please state your use-
case and we will help you judge whether to implement a solution on your own or use our 
services. 
 
This document is intended to provide OEM independent information. If the following explanations do 
not fit with your use-case please do not hesitate to ask for our support. 
2 HIS Flash Driver Interface 
A thorough description of the HIS flash driver interface can be found online. Please check section 0. 
Typically your delivery is going to contain one or more HIS-compliant drivers which can be treated as 
a blueprint for an own implementation. Please check the following folders: 
.\BSW\Fbl\fbl_flio.* 
.\BSW\Flash\flashdrv.* 
.\BSW\Eep 
The flash API consists of the following functions: 
IO_ErrorType FlashDriver_InitSync( void * ); 
IO_ErrorType FlashDriver_DeinitSync( void * ); 
IO_ErrorType FlashDriver_RReadSync( […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
