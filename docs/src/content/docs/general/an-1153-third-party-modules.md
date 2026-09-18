---
title: "AN-ISC-8-1153 Third Party Modules"
sidebar:
  order: 1
---

# AN-ISC-8-1153 Third Party Modules

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Application%20notes-lightgrey)

> **Source:** `Doc/ApplicationNotes/AN-ISC-8-1153_ThirdPartyModules.pdf` — 10 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

**Original metadata:** title `Third Party Modules` · author `Sven Hesselmann`

## What this document covers

How to integrate third-party (non-Vector, e.g. Renesas MCAL) modules into a MICROSAR SIP project.

## Document outline (extracted headings)

- Third Party Modules
- Application Note AN-ISC-8-1153
- Restrictions Customer confidential - Vector decides
- Table of Contents
- 1.0 Overview
- 2.0 Integration in DaVinci Configurator 5
- 2.1 Configuration With CFG5
- 2.1.1 Adding of BSWMD File
- 2.1.2 Adding a Module to the Current Project
- 2.2 External Generation Step
- 2.2.1 Manual Set-Up
- 2.2.2 Automatic Set-Up
- 2.3 Internal Behavior Description
- 2.3.1 Example for Internal Behavior Description

## Key content (extracted text sample)

Third Party Modules 
Version 1.0 
2013-07-24 
Application Note AN-ISC-8-1153 
 
 
 
Author(s) Sven Hesselmann 
Restrictions Customer confidential - Vector decides 
Abstract Introduction how to integrate 3rd partly modules into the MICROSAR4 stack 
 
Table of Contents 
 
 1 
Copyright © 2013 - Vector Informatik GmbH 
Contact Information: www.vector.com or +49-711-80 670-0 
1.0 Overview .......................................................................................................................................................... 1 
2.0 Integration in DaVinci Configurator 5 ............................................................................................................... 2 
2.1 Configuration With CFG5 .............................................................................................................................. 2 
2.1.1 Adding of BSWMD File ............................................................................................................................... 2 
2.1.2 Adding a Module to the Current Project ..................................................................................................... 3 
2.2 External Generation Step .............................................................................................................................. 4 
2.2.1 Manual Set-Up ............................................................................................................................................ 5 
2.2.2 Automatic Set-Up ........................................................................................................................................ 5 
2.3 Internal Behavior Description ........................................................................................................................ 5 
2.3.1 Example for Internal Behavior Description ................................................................................................. 5 
2.3.2 Templates for Internal Behavior Description .............................................................................................. 6 
2.4 RTE configuration .......................................................................................................................................... 7 
2.5 CDD Configuration ........................................................................................................................................ 7 
3.0 Settings.xml ..................................................................................................................................................... 8 
4.0 Integration Into the Build Project ...................................................................................................................... 8 
4.1 Compiler_Cfg.h ............................................................................................................................................. 9 
4.2 MemMap.h .................................................................................................................................................... 9 
5.0 Additional Resources ..................................................................................................................................... 10 
6.0 Contacts ......................................................................................................................................................... 10 
 
 
1.0 Overview 
This application note describes integration of […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
