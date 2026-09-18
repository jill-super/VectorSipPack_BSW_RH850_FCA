---
title: "AN-ISC-8-1196 Distributing BSW Components across Partitions"
sidebar:
  order: 1
---

# AN-ISC-8-1196 Distributing BSW Components across Partitions

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Application%20notes-lightgrey)

> **Source:** `Doc/ApplicationNotes/AN-ISC-8-1196_Distributing_BSW_Components_across_Partitions.pdf` — 7 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

**Original metadata:** title `Distributing BSW Components across Partitions` · author `Wolf, Jonas`

## What this document covers

Distributing BSW components across memory partitions / cores: MemMap, access rights and configuration.

## Document outline (extracted headings)

- Distributing BSW Components across Partitions
- Application  Note  AN-ISC -8-1196
- Table of Contents
- 1 Overview
- Figure 1-1 Basic Software
- 2 Introduction of Partitioning
- 1. Define partitioning scheme
- 2. Identify interfaces between components
- 3. Select technique to implement partition crossing
- Application SWCs
- AUTOSAR Modules
- Complex
- Drivers
- Note

## Key content (extracted text sample)

Distributing BSW Components across Partitions 
Version 1.2 
2017 -05-17 
Application Note AN-ISC -8-1196 
Author Wolf, Jonas 
Restrictions Customer Confidential – Vector decides 
Abstract MICROSAR BSW is supposed to be executed in one memory partition (with some 
exceptions). Architectural constraints, e.g. a safety concept, may require distributing 
MICROSAR BSW across different memory partitions. This application note describes 
the general approach and common techniques for distribution. 
 
 
Table of Contents 
1 Overview ........................................................................................................................................ 2 
2 Introduction of Partitioning .......................................................................................................... 2 
3 Techniques for Crossing Partitions ............................................................................................ 3 
3.1 Trusted Functions ................................................................................................................ 3 
3.2 Non-trusted Functions .......................................................................................................... 3 
3.3 Inter OS Application Communicator (IOC) ........................................................................... 3 
3.4 Sharing Data ........................................................................................................................ 3 
4 Hooking into Interfaces ................................................................................................................ 4 
4.1 Example Code...................................................................................................................... 6 
4.1.1 Source File of A (A\A.c) ....................................................................................................... 6 
4.1.2 Header File of B (B\B.h) ....................................................................................................... 6 
4.1.3 Source File of B (B\B.c) ....................................................................................................... 6 
4.1.4 Header File of Bmod (Bmod\Bmod.h) .................................................................................. 6 
4.1.5 Header File of Bmod (Bmod\B.h) ......................................................................................... 7 
4.1.6 Source File of Bmod (Bmod\Bmod.c) .................................................................................. 7 
5 Additional Resources ................................................................................................................... 7 
6 Contacts ......................................................................................................................................... 7 
 
 
Distributing BSW Components across Partitions 
Copyright © 2017 - Vector Informatik GmbH 2 
Contact Information: www.vector.com or +49-711-80 670-0 
1 Overview 
AUTOSAR was initially developed for single core microcontrollers without memory protection unit 
(MPU). The availability of more powerful microcontrollers and the introduction of ISO 26262 led to new 
concepts in AUTOSAR addressing these changes. 
This document provides an approach how to distribute basic software across partitions on one core. 
Distributing the basic software across different cores is out of scope of this application note. The term 
basic software is used in […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
