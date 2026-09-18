---
title: "AN-ISC-8-1143 Application Validation Strategies"
sidebar:
  order: 1
---

# AN-ISC-8-1143 Application Validation Strategies

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Application%20notes-lightgrey)

> **Source:** `Doc/ApplicationNotes/AN-ISC-8-1143_Application_Validation_Strategies.pdf` — 6 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

**Original metadata:** title `Bootloader Validation Strategies` · author `Achim Strobelt`

## What this document covers

Strategies to validate the application from the bootloader (presence patterns, checksums, secure-boot verification).

## Document outline (extracted headings)

- Bootloader Validation Strategies
- Application Note  AN-ISC-8-1143
- Restrictions Customer confidential - Vector decides
- Table of Contents
- 1.0 Introduction
- 1.1 Scope
- 2.0 Validation Basics
- 2.1 Module Validation
- 2.1.1 Download Integrity
- Note
- 2.1.2 Download Authenticity
- 2.2 Application Validation
- 3.0 Validation Approaches
- 3.1 Pattern

## Key content (extracted text sample)

Bootloader Validation Strategies 
Version 1.0 
2012-03-21 
Application Note AN-ISC-8-1143 
 
 
 
Author(s) Achim Strobelt 
Restrictions Customer confidential - Vector decides 
Abstract This application note describes application validation strategies used in Vector 
Bootloaders. 
 
Table of Contents 
 
 1 
Copyright © 2012 - Vector Informatik GmbH 
Contact Information: www.vector.com or +49-711-80 670-0 
1.0 Introduction ...................................................................................................................................................... 1 
1.1 Scope ............................................................................................................................................................ 1 
2.0 Validation Basics .............................................................................................................................................. 2 
2.1 Module Validation .......................................................................................................................................... 2 
2.1.1 Download Integrity ...................................................................................................................................... 2 
2.1.2 Download Authenticity ................................................................................................................................ 2 
2.2 Application Validation .................................................................................................................................... 3 
3.0 Validation Approaches ..................................................................................................................................... 3 
3.1 Pattern ........................................................................................................................................................... 3 
3.2 Checksum/CRC ............................................................................................................................................. 3 
3.3 Signatures ..................................................................................................................................................... 4 
3.4 Validation Structure ....................................................................................................................................... 4 
4.0 Storage of Validation Information .................................................................................................................... 4 
4.1 EEPROM ....................................................................................................................................................... 4 
4.2 Emulated EEPROM ....................................................................................................................................... 4 
4.3 Presence Patterns ......................................................................................................................................... 5 
5.0 Contacts ........................................................................................................................................................... 5 
 
 
1.0 Introduction 
Today, most automotive ECUs support software download to be able to update the application software or data at 
any time. The Flash Bootloader from Vector provides a convenient way to fulfill this task according to the 
specification of the respective car […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
