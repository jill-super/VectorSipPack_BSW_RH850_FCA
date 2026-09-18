---
title: "Startup Manual FCA SLP5"
sidebar:
  order: 1
---

# Startup Manual FCA SLP5

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-User%20manuals-lightgrey)

> **Source:** `Doc/UserManuals/Startup_FCA_SLP5.pdf` — 195 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).
>
> **Format twin:** the same manual is also shipped as Windows compiled help `Doc/UserManuals/Startup_FCA_SLP5.chm` (13 MB) — identical content, CHM navigation. No separate conversion; refer to this page plus the originals.

**Original metadata:** title `Startup with Vector SLP4` · author `Vector Informatik GmbH (Klaus Emmert, Manuela Huber, Monika Sturm)`

## What this document covers

Step-by-step startup manual for the FCA SLP5 program (ca. 195 pages; also shipped as Startup_FCA_SLP5.chm): install SIP, configure with DaVinci, build DemoFbl/DemoBm, flash and validate on RH850.

## Document outline (extracted headings)

- Content
- 1.1 History Information 11
- 1.2 Finding Information Quickly 11
- 1.3 Conventions 11
- 1.4 Certification 12
- 1.5 Warranty 12
- 1.6 Support 13
- 1.7 Trademarks 13
- 1.8 Errata Sheet of Hardware Manufacturers 14
- 1.9 Example Code 14
- 1.10 What Do You Learn from This Manual 14
- 2.1 An Overall View 16
- 2.2 MICROSAR - Vector's AUTOSAR Solution 17
- 2.3 AUTOSAR Layer Model FCA 17

## Key content (extracted text sample)

Startup with FCA SLP5
Version 6.0.0 for MICROSAR 4 Release 20
© Vector Informatik GmbH Version 6.0.0 for Release 20 - 2-
Content
1AboutThisManual 11
1.1 History Information 11
1.2 Finding Information Quickly 11
1.3 Conventions 11
1.4 Certification 12
1.5 Warranty 12
1.6 Support 13
1.7 Trademarks 13
1.8 Errata Sheet of Hardware Manufacturers 14
1.9 Example Code 14
1.10 What Do You Learn from This Manual 14
2Basics 16
2.1 An Overall View 16
2.2 MICROSAR - Vector's AUTOSAR Solution 17
2.3 AUTOSAR Layer Model FCA 17
ISTEPbySTEP 19
1STEP1SetupYourProject 20
1.1 Situation after Installation 20
1.1.1 Vector AUTOSAR XML Editor- A Useful Tool 20
1.2 Setup Project via DaVinci Configurator Pro 21
1.2.1 General Settings 22
1.2.2 Project Folder Structure 22
1.2.3 Target 22
1.2.4 DaVinci Developer 23
1.2.5 Creating DaVinci Developer Workspace later 23
1.3 Result Project Folder - Result of the Project Setup 25
1.3.1 Appl folder 25
1.3.2 Config folder 25
1.3.3 <ProjectName>.dpa 26
1.3.4 Log Folder 26
Content User Manual Startup with FCA SLP5
1.4 Start Menu - Result of the Project Setup 27
1.5 DaVinci Configurator Pro Project 27
2STEP2DefineProjectSettings 28
2.1 Add Input Files 28
2.1.1 Input File Assistant 28
2.1.2 Add System Description Files 29
2.1.3 Add Diagnostic Data Files 30
2.1.4 Define Options for Input Files 32
2.1.5 Update Configuration 32
2.2 Define External Generation Steps and SWC Templates and Contract Phase Headers 35
2.2.1 External Generation Steps 35
2.2.2 SWC Templates and Contract Phase Headers 36
2.3 Activate Your BSW Modules 37
2.4 Add ECUC File References 38
2.5 Change Project Settings 38
2.5.1 Postbuild Support 38
3STEP3Validation 40
3.1 Start Solve All Mechanism 40
3.2 Live Validation - Solving Actions 40
4STEP4StartBSWConfiguration 42
4.1 Start Configuration with Configuration Editors 42
4.2 Base Services 42
4.2.1 Default Error Tracer 42
4.2.2 General Purpose Timer (GPT) 42
4.2.3 RAM Test 42
4.3 Communication 43
4.3.1 Communication General 43
4.3.2 Bus Controller 43
4.3.3 PDUs 44
4.3.4 Signals 44
© Vector Informatik GmbH Version 6.0.0 for Release 20 - 3-
Content User Manual Startup with FCA SLP5
© Vector Informatik GmbH Version 6.0.0 for Release 20 - 4-
4.3.5 Socket Adapter Users 44
4.4 Diagnostics 44
4.4.1 Diagnostic Data Identifiers 44
4.4.2 Diagnostic Event Data 45
4.4.3 Diagnostic Events 45
4.4.4 Production Error Handling 45
4.4.5 Add Diagnostic Data ID Assistant 45
4.4.6 Automap Diagnostic Data Objects 46
4.4.7 Setup Event Memory Blocks 46
4.5 I/O 46
4.5.1 IO Hardware Abstraction 46
4.6 Memory 47
4.6.1 Memory General 47
4.6.2 Memory Blocks 47
4.6.3 Optimize Fee 47
4.7 Mode Management Editors 47
4.7.1 BSW Management 47
4.7.2 Activate Interrupts of Peripherals Devices 50
4.7.3 ECU Management 53
4.7.4 Initialization 53
4.7.5 Watchdogs 53
4.8 Network Management 54
4.8.1 Partial Networking 54
4.9 Runtime System 54
4.9.1 Runtime System General 54
4.9.2 ECU Software Components 54
4.9.3 Module Internal Behavior 55
4.9.4 OS Configuration 55
4.9.5 Task Mapping 56
4.10 Go on with Basic Editor 56
Content User Manual Startup with FCA SLP5
4.11 Start Solving Actions 56
4.12 Start On-demand Validation 56
4.13 BSW Configuration finished 58
5STEP5DesignSoftwareComponents 59
5.1 Switch to DaVinci Developer 59
5.2 Design Software Components 60
6STEP6Mappings 61
6.1 Perform Data Mapping within DaVinci Developer or DaVinci Configurator? 61
6.2 Data Mapping within the DaVinci Developer 61
6.2.1 Data Mapping Automatically - DaVinci Developer […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
