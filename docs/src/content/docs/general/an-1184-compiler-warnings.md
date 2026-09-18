---
title: "AN-ISC-8-1184 Compiler Warnings"
sidebar:
  order: 1
---

# AN-ISC-8-1184 Compiler Warnings

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Application%20notes-lightgrey)

> **Source:** `Doc/ApplicationNotes/AN-ISC-8-1184_Compiler_Warnings.pdf` — 8 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

**Original metadata:** title `Compiler Warnings` · author `Andreas Raisch`

## What this document covers

How to interpret and handle compiler warnings reported for Vector BSW sources.

## Document outline (extracted headings)

- Compiler Warnings
- Application  Note  AN-ISC -8-1184
- Author Andreas Raisch
- Table of Contents
- 1 Overview
- Figure 1 MICROSAR BSW Component
- 1.1 Deviation Procedure
- Priority Rule Rationale
- MICROSAR BSW shall be compiler
- Detection of compiler warning either during
- We want to prevent to deliver defect code to
- If fixing the compiler warning is not a
- See list of accepted deviations in this
- Table 1 Priority of measures to prevent compiler warnings

## Key content (extracted text sample)

Compiler Warnings 
Version 1.0 
2015 -11-02 
Application Note AN-ISC -8-1184 
Author Andreas Raisch 
Restrictions Customer confidential – Vector decides 
Abstract Warning free code is an important quality goal for embedded software. Nevertheless, 
compiler warnings can occur for highly configurable software. Typical compiler 
warnings are listed and justified within this document. 
 
 
Table of Contents 
1 Overview ........................................................................................................................................ 2 
1.1 Deviation Procedure ............................................................................................................ 3 
1.2 Default BSW Delivery Process ............................................................................................ 3 
2 Accepted Deviations ..................................................................................................................... 3 
2.1 Unused/unreferenced parameter/argument ......................................................................... 4 
2.2 Unused/unreferenced define, enum value ........................................................................... 4 
2.3 Unused/unreferenced variable ............................................................................................. 4 
2.4 Unused/unreferenced function ............................................................................................. 5 
2.5 Condition evaluates always to true/false ............................................................................. 5 
2.6 Unreachable code/statement ............................................................................................... 6 
2.7 Dead assignment / variable set but not used ....................................................................... 6 
2.8 ASM statements used .......................................................................................................... 6 
3 Additional Resources ................................................................................................................... 7 
4 Contacts ......................................................................................................................................... 8 
 
 
Compiler Warnings 
 
Copyright © 2015 - Vector Informatik GmbH 2 
Contact Information: www.vector.com or +49-711-80 670-0 
1 Overview 
MICROSAR BasicSoftware (BSW) is developed in a product line approach, independent from specific 
ECU projects or compilers. MICROSAR BSW supports the AUTOSAR MemoryAbstraction and 
CompilerAbstraction concepts and supports a huge range of different compiler vendors, versions and 
options. 
MICROSAR BSW is delivered as static source code and code generators to support the ECU project 
specific adaption and optimization of the BSW behavior and feature set based on AUTOSAR 
configuration files and user defined selections. 
Additionally, MICROSAR BSW supports compile time configuration, link time configuration and post-
build configuration. 
 
Figure 1 MICROSAR BSW Component 
A general quality goal for MICROSAR BSW is “warning free code”. The coding style guide for 
MICROSAR BSW is based on MISRA-C:2004. Checks for MISRA compliance are an essential part of 
our development process. Based on “HIS Gemeinsames Subset der MISRA C Guidelines v2.0“ 
(http://www.automotive-his.de) all rules are active. 
Nevertheless, we accept deviations to the “warning free code” goal based on […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
