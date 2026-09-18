---
title: "Mcal_Rh850P1xC"
sidebar:
  order: 1
---

# Mcal_Rh850P1xC
![Third-party](https://img.shields.io/badge/Third-party-red) ![Layer](https://img.shields.io/badge/layer-mcal-lightgrey)
> **Origin:** Third-party (Renesas MCAL, not delivered). Third-party Renesas MCAL integration point — the MCAL itself is NOT shipped with this SIP.
## Purpose

Integration point for the Renesas RH850 P1x-C MCAL (ADC, DIO, FLS, MCU, PORT, SPI, WDG, GPT, ICU, PWM, ...). Only Vector .mak integration files and BSWMD references are shipped; the MCAL itself must come from Renesas. See the 3rd-party MCAL integration references.
## Responsibility

Declares the expected Renesas MCAL surface; no MCAL sources are shipped.
## Key files

No C sources shipped in this SIP slice (integration/`.mak`-only module). See the page notes and linked documents.

Build fragments: `mak/Mcal_Rh850P1xC_cfg.mak`, `mak/Mcal_Rh850P1xC_check.mak`, `mak/Mcal_Rh850P1xC_defs.mak`, `mak/Mcal_Rh850P1xC_rules.mak`

## Public API (excerpt from headers)

No exported C API surface detected (types/macros/templates only) — see headers and templates in the file list.

## Usage example

See the linked Technical Reference and the `Demo` integration (`Demo/DemoFbl/Appl/Source/fbl_ap*.c`) for call sequences.

## Dependencies

`_Common`, `MakeSupport`

## Converted Vector documents

- [TechnicalReference_3rdParty-MCAL-Integration](mcal_rh850p1xc-3rdparty-mcal-integration/) (source: `Doc/TechnicalReferences/TechnicalReference_3rdParty-MCAL-Integration.pdf`)
- [TechnicalReference_3rdParty-MCAL-Integration_P1x-C](mcal_rh850p1xc-3rdparty-mcal-integration-p1x-c/) (source: `Doc/TechnicalReferences/TechnicalReference_3rdParty-MCAL-Integration_P1x-C.pdf`)
