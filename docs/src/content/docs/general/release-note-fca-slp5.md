---
title: "Release Note FCA SLP5"
sidebar:
  order: 1
---

# Release Note FCA SLP5

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Release%20notes-lightgrey)

> **Source:** `Doc/ReleaseNotes/ReleaseNote_FCA_SLP5.pdf` — 67 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

**Original metadata:** title `Release Notes FCA SLP5` · author `Vector Informatik GmbH (Klaus Emmert, Manuela Huber, Monika Sturm)`

## What this document covers

Customer-facing release notes for the FCA SLP5 bootloader delivery (FBL FCA SLP5): content of the release, changes, open issues and integration hints.

## Document outline (extracted headings)

- Release Notes
- FCA SLP5
- Content
- 1 Release 20 4
- General 4
- Communication 4
- Diagnostics 8
- Ethernet 12
- Gateway 14
- J1939 18
- Measurement and Calibration 18
- Runtime 18
- Security 19
- State Management 20

## Key content (extracted text sample)

Release Notes
FCA SLP5
Content
1 Release 20 4
General 4
Communication 4
Diagnostics 8
Ethernet 12
Gateway 14
Inter Process Communication (IPC) 14
J1939 18
Measurement and Calibration 18
Runtime 18
Security 19
State Management 20
V2G 21
vVIRTUALtarget 21
Watchdog 22
Tooling 22
2 Release 19 43
General 43
Communication 43
Diagnostics 43
Ethernet 47
FCA SLP5 | Release Notes

Gateway 47
IPC 48
J1939 48
Measurement and Calibration 49
Nv Memory 52
Rte 53
Security 55
Time Synchronization 56
V2G 58
Tooling 59
FCA SLP5 | Release Notes

1 Release 20
General
Type Description Change ID
Information Several MICROSAR BSW modules make use of float datatypes. The usage of a "nofloat" compiler option is there-
fore no longer supported.
-
Communication
Type Description Change ID
Breaking
Change
The time synchronization stack has been extended with more AR4.3 features:
> StbM now supports
> Virtual local time: Rate correction based on the network time
> Pure local time base: Time base derived from a local clock / counter
> New API StbM_GetTimeBaseStatus()
> StbM_SetGlobalTime() can now also be used for offset time bases
> CanTSyn and FrTSyn now support the AR4.3 defined message format which is incompatible to the message
format defined by AR4.2.2.
> The message format is configurable to support OEMs that require AR4.2.2 message format on the net-
work.
> EthTsyn is now able to detect Master / Slave conflicts.
> The slave node reports runtime DET error if SYNC messages from multiple master nodes are received.
> The slave node detects the first Master and ignores messages from other master nodes.
> The master node reports a runtime DET error if SYNC messages are received from other master nodes.
Migration notes for existing projects:
If the OEM requires time synchronization according AR4.2.2 (message format) set the configuration parameter
CanTSynMessageCompatibility resp. FrTSynMessageCompatibility to TRUE.
FEAT-2461
FCA SLP5 | Release Notes
General

Type Description Change ID
Additional Information
Typically Vector will preconfigure this item according to the OEM the SIP has been ordered for.
Breaking
Change
The MICROSAR COM Stack is now able to handle PDU fan-outs in the PduR. This reduces resource consumption
in the Com module as the signals exists only once even if being transmitted on multiple networks.
The PDU fan-out must be modelled in the system template.
Important Information
In order to realize this feature the naming rules of the upstream mapping have been changed.
> Names of PDUs and signals that are created by DaVinci Configurator Pro based on the System
Template are changed during the first database update.
> Due to internal improvement in our tooling there have also been other changes with respect to
names that are created by the upstream mapping (System Extract -> EcuC).
The implementation has some limitations
> If a Com I-PDU Group is assigned only to PDUs with a fan-out or fan-in relation the BswM is cur-
rently not able to switch these PDU groups based on the rules created by the auto configuration.
> This is a absolutely untypical use-case and we are currently not aware that such databases
are provided by OEMs.
> Enabling and disabling these PDU Groups have to be done manually in the BswM configuration
as otherwise the PDUs will not be processed. Future release will improve this handling.
Migration notes for existing projects:
Due to the fan-out/fan-in realization and due to the associated renaming of items we have a high impact on […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
