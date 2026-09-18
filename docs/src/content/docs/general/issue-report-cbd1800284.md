---
title: "Issue Report CBD1800284"
sidebar:
  order: 1
---

# Issue Report CBD1800284

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Delivery%20information-lightgrey)

> **Source:** `Doc/DeliveryInformation/IssueReport_CBD1800284.pdf` — 110 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

## What this document covers

Full issue report (ca. 110 pages, incl. XML variant IssueReport_CBD1800284.xml): all known issues / ESCAN entries valid for this delivery.

## Document outline (extracted headings)

- Issue Report
- License Number Customer
- CBD1800284 Nexteer Automotive Corporation
- Automotive company with Full RScan
- Maintenance Expiry Date
- SIP Version
- SLP Delivery Number
- FBL Fca SLP5 D00
- Report Creation Date
- Contact
- Table of Contents
- 1. Introduction
- 1.1 Resolving Issues
- 1.2 Issue Classification

## Key content (extracted text sample)

Issue Report
1
License Number Customer
CBD1800284 Nexteer Automotive Corporation
Package: FBL Fca SLP5 - the company Nexteer 
Automotive company with Full RScan
Maintenance Expiry Date
2018-09-01
SIP Version
20.07.00
SLP Delivery Number
FBL Fca SLP5 D00
Report Creation Date
2018-08-03
Contact
In case of questions or the need for an update of the basic software delivery, please contact 
Support@vector.com or your Vector contact person.
Table of Contents
1. Introduction
1.1 Resolving Issues
1.2 Issue Classification
2. New Issues
2.1 Safety Relevant Issues: 3
2.2 Runtime Issues without Workaround: 3
2.3 Runtime Issues with Workaround: 8
2.4 Not Released Functionality: 7
2.5 Apparent Issues: 52
2.6 Compiler Warnings: 29
3. New Issues for Information: 0
4. Report Legend
5. 3rd Party Software Issues
6. Quality Management Contact
Issue Report
2
1. Introduction
1.1 Resolving Issues
Reported issues are not automatically fixed with the next update delivery.
If a reported issue shall be fixed, please contact Vector agree on the issues that can be fixed with 
upcoming deliveries. 
Please note that Vector may fix issues without explicit request.
1.2 Issue Classification
This Issue Report provides issues that have been detected since the last report. The issues have 
been classified to facilitate the assessment of their impact:
The chapter 'New Issues' lists issues that have been detected since the last report and which could 
not be excluded based on the use-case defined in the questionnaire. The issues are classified as 
follows:
• Safety Related Issues: Safety related issues have impact on the functional safety of the 
software module. If this issue interferes with the functional safety concept of the ECU, this 
module (or module configuration) must not be used for serial production in a safety-related 
project. The effect of the issue to the ECU functionality and functional safety has to be 
analyzed by the user as the software usage and its configuration is not known by Vector. The 
risk of change has also to be taken into account.
• Runtime Issues without Workaround: Runtime issues without a workaround require an 
update of the software delivery in case the issue affects the ECU overall functionality. The 
effect of an issue to the ECU functionality has to be analyzed by the customer as the software 
usage and its configuration is not known by Vector. The risk of change has also to be taken 
into account.
• Runtime Issues with Workaround: It is not recommended to update a delivery due to a 
runtime issue with a documented workaround. The effect of an issue to the ECU functionality 
has to be analyzed by the user as the software usage and its configuration is not known by 
Vector. The risk of change has also to be taken into account.
• Not Released Functionality: Not released functionalities (BETA) are either complete 
software modules or features in the software module that have not yet passed a complete 
development cycle (they are e.g. not or only partly tested). If a BETA issue ticket affects a 
complete software module, the software module must not be used for serial production. If a 
BETA issue ticket affects a feature in the software module, the user has to ensure that all 
BETA features are disabled as indicated for the serial production release of the ECU.
• Apparent Issues: Apparent issues are detected immediately when using the software 
module. If an issue does not show up while working with the software module, the ECU 
project is […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
