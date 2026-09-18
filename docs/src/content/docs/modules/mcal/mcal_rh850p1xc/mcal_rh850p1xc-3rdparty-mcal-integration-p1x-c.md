---
title: "Converted: 3rd-Party MCAL Integration P1x-C"
sidebar:
  order: 2
---

# Converted: Technical Reference — 3rd-Party MCAL Integration P1x-C

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_3rdParty-MCAL-Integration_P1x-C.pdf` — 9 pages · original title `MICROSAR [BSW module]`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **3rd-Party MCAL Integration P1x-C**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- Technical Reference
- Renesas RH850 P1M-C/P1H-C/P1H-CE
- Authors Andrej Gazvoda
- Status Released
- Technical Reference 3rdParty MCAL Integration
- Document Information
- History
- Author Date Version Remarks
- Reference Documents
- Scope of the Document
- Contents
- 2.1.1.1 Spi Module cannot be generated ................................ ..... 6
- 2.1.1.2 Fls Module Generation Mismatch ................................ ..... 6
- 2.1.2.1 Spi: Generation error regarding SpiClockFrequencyRef .. 6

## Key content (extracted text sample)

3rdParty MCAL Integration 
Technical Reference 
 
Renesas RH850 P1M-C/P1H-C/P1H-CE 
Version 1.0.0 
 
 
 
 
 
 
 
 
 
 
 
Authors Andrej Gazvoda 
Status Released 
 
 
 
 
 
Technical Reference 3rdParty MCAL Integration 
© 2018 Vector Informatik GmbH Version 1.0.0 2 
based on template version 6.0.1 
Document Information 
History 
Author Date Version Remarks 
Andrej Gazvoda 2018-06-08 1.0.0 Initial revision 
 
Reference Documents 
No. Source Title Version 
[1] Vector TechnicalReference_3rdParty-MCAL-Integration.pdf see delivery 
 
Scope of the Document 
This document contains information about the integration of 3 rd Party MCAL into Vector 
software stack. 
Technical Reference 3rdParty MCAL Integration 
© 2018 Vector Informatik GmbH Version 1.0.0 3 
based on template version 6.0.1 
Contents 
1 MCAL Integration ................................ ................................ ................................ .......... 4 
1.1 Type of Integration ................................ ................................ ............................. 4 
1.2 MCAL Location within SIP ................................ ................................ .................. 4 
1.3 Supported 3rd Party Products ................................ ................................ ............. 4 
1.4 Configuration Tools ................................ ................................ ............................ 5 
2 Vector Comment ................................ ................................ ................................ ........... 6 
2.1 Known Issues ................................ ................................ ................................ .... 6 
2.1.1 Ver4.02.00 ................................ ................................ ......................... 6 
2.1.1.1 Spi Module cannot be generated ................................ ..... 6 
2.1.1.2 Fls Module Generation Mismatch ................................ ..... 6 
2.1.2 Ver4.02.01 ................................ ................................ ......................... 6 
2.1.2.1 Spi: Generation error regarding SpiClockFrequencyRef .. 6 
2.1.2.2 Spi: Generation error regarding SpiEnableCs .................. 7 
2.1.2.3 Generation error regarding FlsCpuFrequency .................. 7 
3 Glossary and Abbreviations ................................ ................................ ........................ 8 
3.1 Glossary ................................ ................................ ................................ ............ 8 
3.2 Abbreviations ................................ ................................ ................................ ..... 8 
4 Contact ................................ ................................ ................................ .......................... 9 
 
Technical Reference 3rdParty MCAL Integration 
© 2018 Vector Informatik GmbH Version 1.0.0 4 
based on template version 6.0.1 
1 MCAL Integration 
1.1 Type of Integration 
 
Comfort Integration 
Vector tool DaVinci Configurator 5 is used for configuration 
 
> as comfort editor for Mcu component (clock tree) 
> as generic editor for other MCAL modules 
 
Recommended workflow: 
Generation and changes in configuration are done in DaVinci Configurator. 
1.2 MCAL Location within SIP 
 
The 3 rd Party MCAL is separated from the Vector parts within the SIP. Furthermore, it 
might not be part of the delivery. In this case please refer to chapter ‘First Steps’ in 
document TechnicalReference_3rdParty-MCAL-Integration.pdf [1]. 
 
1.3 Supported 3rd Party Products 
This integration supports the following Renesas targets: 
 
 RH850P1M-C 
 RH850P1H-C 
 RH850P1H-CE 
 
 
 
Note 
Please refer to the Release Notes of the 3rd Party Products for further 
information, e.g. regarding supported versions, derivatives and compilers. 
 
 
 
 
 
Note 
Please be aware that only official 3rdParty-Vendor releases are part of this Vector 
integration package. Therefore any customer-specific releases cannot be considered. 
 
 

Technical Reference 3rdParty MCAL Integration 
© 2018 Vector Informatik GmbH Version 1.0.0 5 
based on template version 6.0.1 
 
 
Caution 
Please contact the 3rdPartyVendor to find out if there are further Hotfixes 
available for your Mcal package. 
It is essential to replace the affected MCAL parts in your original package 
before you start Script_MCAL_Prepare.bat. 
 
 
1.4 Configuration Tools 
> DaVinci Configurator 5 
 
 

Technical Reference 3rdParty MCAL Integration 
© 2018 Vector […]

## Related module

See [Mcal_Rh850P1xC](../) for purpose, API, files and dependencies.
