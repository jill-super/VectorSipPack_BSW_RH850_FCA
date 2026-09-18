---
title: "Converted: 3rd-Party MCAL Integration"
sidebar:
  order: 2
---

# Converted: Technical Reference — 3rd-Party MCAL Integration

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_3rdParty-MCAL-Integration.pdf` — 34 pages · original title `MCAL Integration Package`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **3rd-Party MCAL Integration**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MCAL Integration Package
- Technical Reference
- Basics and workflows
- Wuttke
- Status Released
- Technical Reference MCAL Integration Package
- Document Information
- History
- Author Date Version Remarks
- Known Issue for missing
- AUTOSAR use case
- MCAL preparation
- Integration video
- Reference to QuickStart

## Key content (extracted text sample)

MCAL Integration Package 
Technical Reference 
 
Basics and workflows 
Version 1.05.01 
 
 
 
 
 
 
 
 
 
 
Authors Andrej Gazvoda, Günther Piehler, Roland Süß, Ingo 
Wuttke 
Status Released 
 
 
 
 
 
Technical Reference MCAL Integration Package 
© 2018 Vector Informatik GmbH Version 1.05.01 2 
based on template version 5.2.0 
Document Information 
History 
Author Date Version Remarks 
Roland Süß; Ingo Wuttke 2015-02-27 1.00.00 Initial Ideas, usage as 
Application Note; Porting to 
Technical Reference 
template; adding detailed 
description about 3rd party 
tools etc. 
Günther Piehler 2015-04-24 1.00.01 Review; small changes to 
increase understandability; 
Known Issue for missing 
config items added  
released 
Andrej Gazvoda; Roland Süß 2015-06-30 1.00.02 7.3 / 7.4 - Added known 
issues regarding EB tresos™ 
tool 
Günther Piehler 2015-07-17 1.01.00 2.3 - Introduction of Mixed 
AUTOSAR use case 
3 ff - Extend description of 
MCAL preparation 
(prerequisites) 
4 - hint about recommended 
workflow added 
Günther Piehler 2015-10-26 1.01.01 3.2.2 / 3.2.3 - parameter 
corrected 
4 – added hint for MCAL 
Integration video 
Günther Piehler 2016-01-26 1.02.00 4.2 - added hint for “round 
trip” ability 
general - new CI applied 
Günther Piehler 2016-07-05 1.03.00 Page 3 - Added further useful 
documents as reference 
 
Günther Piehler 2016-09-27 1.04.00 1 – completely new 
Reference to QuickStart 
document deleted (replaced 
within this document); 
Reference to ScreenCase 
and ReleaseNote added 
Hints for AUTOSAR3 <-> 
AUTOSAR4 differentiation 
added 
3.2.2 – non-interactive mode 
introduced 
3.2.3 – reference to Release 
Notes added for further info 
Technical Reference MCAL Integration Package 
© 2018 Vector Informatik GmbH Version 1.05.01 3 
based on template version 5.2.0 
6 – completely new 
7 – issue for “MCAL and SIP 
storage location” removed 
8 – hint to “generate all” 
added 
Roland Süß 2017-11-09 1.05.00 3 - Adapted chapter: Details 
regarding 3rd party MCAL 
Integration Helper 
4.2 - Adapted Chapter: "Set 
User Defined" Action 
5.3 - Added chapter 
5.5 - Added chapter 
 
Roland Süß 2018-04-27 1.05.01 5.3 - Extended chapter 
Reference Documents 
No. Source Title Version 
[1] Vector Product Information MICROSAR Vector SLP4 1.03.02 
[2] Vector Catalog – Product Information MICROSAR – Chapter MCAL V1.3 – 
2015-02 
[3] Vector Application Note “AN-ISC-8-1153_ThirdPartyModules.pdf” Latest 
(e.g. 1.0) 
[4] Vector Application Note “AN-ISC-8-1171_Tresos_LicenseHandling.pdf” Latest 
(e.g. 
1.00.01) 
[5] Vector Application Note “AN-ISC-8-1180_MCAL-Integration-Variants.pdf” Latest 
(e.g. 0.9) 
[6] Vector Release Note 
“ReleaseNotes_3rdPartyMCAL_VectorIntegration.pdf” 
As 
provided 
within 
your SIP 
[7] Vector ScreenCast_McalIntegration_Tresos.pdf As 
provided 
within 
your SIP 
[8] Vector Technical Reference 
"TechnicalReference_3rdParty-MCAL-
Integration_<controller>.pdf" 
As 
provided 
within 
your SIP 
 
 
Technical Reference MCAL Integration Package 
© 2018 Vector Informatik GmbH Version 1.05.01 4 
based on template version 5.2.0 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 

Technical Reference MCAL Integration Package 
© 2018 Vector Informatik GmbH Version 1.05.01 5 
based on template version 5.2.0 
Contents 
1 Purpose of the document ................................ ................................ ............................. 8 
2 Introduction................................ ................................ ................................ ................... 9 
2.1 Responsibility ................................ ................................ ................................ ..... 9 
2.2 Support requests................................ ................................ .............................. 10 
2.3 Mix between AUTOSAR specification versions ................................ ................ 10 
3 First Steps ................................ ................................ ................................ ................... 11 
3.1 Delivery structure ................................ ................................ ............................. 11 
3.2 Starting up […]

## Related module

See [Mcal_Rh850P1xC](../) for purpose, API, files and dependencies.
