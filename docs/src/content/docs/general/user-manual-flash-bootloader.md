---
title: "User Manual Flash Bootloader"
sidebar:
  order: 1
---

# User Manual Flash Bootloader

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-User%20manuals-lightgrey)

> **Source:** `Doc/UserManuals/UserManual_FlashBootloader.pdf` — 56 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

**Original metadata:** title `User Manual` · author `Klaus Emmert`

## What this document covers

Hands-on user manual for the Vector Flash Bootloader: concepts, integration workflow and getting-started steps.

## Document outline (extracted headings)

- Flash Bootloader
- User Manual
- User Manual  Flash Bootloader
- CAN LIN
- History
- Author Date Version Remarks
- New symbols
- Motivation For This Work
- WARNING
- A short story
- Contents
- 1.1 Beginners with Flash Bootloader start here ? ..................................... 7
- 2.2 Legend and Explanation of Symbols................................................. 10
- 3.8 What The Flash Bootloader NOT Does ............................................ 15

## Key content (extracted text sample)

Vector Informatik GmbH, Ingerheimer Str. 24, 70499 Stuttgart 
Tel. 0711/80670-0, Fax 0711/80670-399, Email can@vector-informatik.de 
Internet http:\\www.vector-informatik.de 
 
 
 
 
 
 
 
 
 
 
 
Flash Bootloader 
User Manual 
(Your First Steps) 
 
 
Version 2.7 
 
 
 
 
 
 
 
User Manual Flash Bootloader 
1/ 5 6
 
 
 
 
 
 
CAN LIN
 
 
 
 
 
 
 
 
 
 
Authors: Klaus Emmert 
Version: 2.7 
Status: released (in preparation/completed/inspected/released) 
 
 
 
 
 
©2006, Vector Informatik GmbH Version: 2.7 
 based of template version 2.0 
User Manual Flash Bootloader 
2/ 5 6
History 
Author Date Version Remarks 
Klaus Emmert 2004-07-09 2.2 Switch to new Layout Version 2.0 
New symbols 
Klaus Emmert 2004-02-09 2.3 Changes from Review Ra 2004-
09-20, link labels 
Klaus Emmert 2005-03-23 2.4 Chapter 3.8 and warning for 
startup-codes added 
Klaus Emmert 2006-02-06 2.5 Change of file structure 
Klaus Emmert 2006-08-18 2.6 File Structure illustration 
Klaus Emmert 2006-09-01 2.7 WDtimer and some minor issues 
©2006, Vector Informatik GmbH Version: 2.7 
 based of template version 2.0 
User Manual Flash Bootloader 
3/ 5 6
Motivation For This Work 
After a seemingly almost endlessly long development process, the software is 
finally finished and ready for the ECU, downloaded one last time, tested and the 
ECUs packaged for express delivery the next day. 
Now it‘s 10:00 P.M. 
Shortly before quitting time the next busi ness day the telephone rings, and what is 
on the display makes your forehead break out in a sweat of alarm! Errors, nothing 
is working, says the message from your customer. You hastily start up another 
ECU in the lab and you have to also observe the same result just reported to you. 
After searching for a little while you realize that the error is in version management. 
You put the correct version together, recompile it, briefly test the result and send 
the hex code to your customer, who can now flash the new functioning software via 
CAN and diagnostics onto the ECU and as a result, can proceed with the planned 
tests without substantial delays. 
 
 
 
 
 
 
 
 
 
 
 
WARNING 
All application code in any of the Vector User Manuals is for training 
purposes only. They are slightly tested and designed to understand the basic 
idea of using a certain component or a set of components. 
A short story 
about flashing
©2006, Vector Informatik GmbH Version: 2.7 
 based of template version 2.0 
User Manual Flash Bootloader 
4/ 5 6
Contents 
1 Welcome to the Flash Bootloader User Manual ............................................. 7 
1.1 Beginners with Flash Bootloader start here ? ..................................... 7 
1.2 For Advanced Users ........................................................................... 7 
1.3 Special topics ...................................................................................... 7 
1.4 Documents this one refers to… ........................................................... 8 
2 About This Document ....................................................................................... 9 
2.1 How This Documentation Is Set-Up .................................................... 9 
2.2 Legend and Explanation of Symbols................................................. 10 
3 Flashing – An Overall View ............................................................................ 11 
3.1 What Is Flashing? ............................................................................. 11 
3.2 What […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
