---
title: "AN-ISC-8-1149 ErrorHook / E_OS_DISABLED_INT"
sidebar:
  order: 1
---

# AN-ISC-8-1149 ErrorHook / E_OS_DISABLED_INT

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Application%20notes-lightgrey)

> **Source:** `Doc/ApplicationNotes/AN-ISC-8-1149_ErrorHook_E_OS_DISABLED_INT.pdf` — 4 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

## What this document covers

Handling of the E_OS_DISABLED_INT error hook scenario in Vector BSW/OS environments.

## Document outline (extracted headings)

- Application Note  AN-ISC-8-1149
- Restrictions Customer confidential - MSR4 only
- Table of Contents
- 1.0 Overview
- 1.1 Problem Description
- 2.0 Solution
- 2.1 Do Not Use OS Timer
- This API can either
- 2.2 Do Not Lock Global Interrupts
- 3.0 Contacts
- Germany
- Vector Informatik GmbH
- 70499 Stuttgart
- GERMANY

## Key content (extracted text sample)

Avoid ErrorHook E_OS_DISABLED_INT 
Version 1.0 
2015-03-13 
Application Note AN-ISC-8-1149 
 
 
 
Author(s) Birke, Holger 
Restrictions Customer confidential - MSR4 only 
Abstract This application note describes how to avoid ErrorHook E_OS_DISABLED_INT 
 
Table of Contents 
 
 1 
Copyright © 2015 - Vector Informatik GmbH 
Contact Information: www.vector.com or +49-711-80 670-0 
1.0 Overview .......................................................................................................................................................... 1 
1.1 Problem Description ...................................................................................................................................... 1 
2.0 Solution ............................................................................................................................................................ 1 
2.1 Do Not Use OS Timer ................................................................................................................................... 1 
2.2 Do Not Lock Global Interrupts ....................................................................................................................... 3 
3.0 Contacts ........................................................................................................................................................... 4 
 
 
1.0 Overview 
This note describes how to avoid the issue E_OS_DISABLEDINT notified by the OS ErrorHook() callout. 
 
1.1 Problem Description 
The CAN Driver uses the OS APIs GetCounterValue() and GetElapsedValue() to handle asynchronous 
state transitions. These calls will be done out of the context of Can_SetControllerMode() within some 
EXCLUSIVE_AREA from: 
 CAN Driver (CAN_EXCLUSIVE_AREA_6) 
 CAN Interface (CANIF_EXCLUSIVE_AREA_0) 
 CANSM (CANSM_ EXCLUSIVE_AREA_1, CANSM_ EXCLUSIVE_AREA_4) 
 COMM (COMM_ EXCLUSIVE_AREA_1) 
 
If the integrator choose Global Interrupt Lock for these EXCLUSIVE_AREAs the OS will issue 
E_OS_DISABLEDINT by the ErrorHook() callout. 
Note: The issue only appears when you use Global Interrupt Lock for particular EXCLUSIVE_AREA. 
 
2.0 Solution 
There are different solutions for this problem. The integrator has to decide which one fits best to the project-specific 
needs. The descriptions of the EXCLUSIVE AREA have to be checked for limitations. 
2.1 Do Not Use OS Timer 
When the above described AREAs have to use Global Interrupt Lock, no OS timer can be used. Use the 
CAN Driver feature instead. 
 Avoid ErrorHook E_OS_DISABLED_INT 
 
 
 
 2 
Application Note AN-ISC-8-1149 
 
 
Figure 1 – GENy: Hardware Loop Check by Application 
 
 
Figure 2 –DaVinci Configurator: Hardware Cancel By Appl. 
 
This feature provides an additional API called instead of the OS timer and has to be implemented by the integrator. 
Refer to the CAN Driver Technical Reference for detailed description of the API. 
This API can either 
 Use free running timer or 
 Use counter loop (wait dedicated amount of loop calls to secure timing) 
 
Attention: This additional API is called for every Hardware Loop, not only for state transitions. So the worst 
case scenario has to be taken into account for timeout (see CAN Driver Technical Reference) 
 

 Avoid ErrorHook E_OS_DISABLED_INT 
 
 
 
 3 
Application Note AN-ISC-8-1149 
 
2.2 Do Not Lock Global Interrupts 
It is possible to use a user defined callback function to handle the EXCLUSIVE AREAs. 
 
Figure 3 – DaVinci Configurator […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
