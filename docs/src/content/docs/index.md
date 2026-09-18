---
title: BSW RH850 FCA
template: splash
hero:
  title: BSW RH850 FCA
  tagline: Vector MICROSAR Flash Bootloader SIP (CBD1800284) for Renesas RH850 — FCA SLP5. AUTOSAR BSW documentation, module references and converted Vector documents.
  actions:
    - text: Vector SIP overview
      link: /sip/
      icon: right-arrow
    - text: Modules by layer
      link: /modules/
      icon: open-book
    - text: General documents
      link: /general/
      icon: document
---

![Platform](https://img.shields.io/badge/platform-Renesas%20RH850-blue)
![Language](https://img.shields.io/badge/language-C-orange)
![License](https://img.shields.io/badge/license-MIT-green)
![AUTOSAR](https://img.shields.io/badge/AUTOSAR-Classic%20BSW-lightgrey)
![SIP](https://img.shields.io/badge/SIP-CBD1800284-purple)

Vector MICROSAR **Flash Bootloader Software Integration Package (SIP) CBD1800284** for the
**FCA SLP5** program (customer: Nexteer), targeting **Renesas RH850** derivatives
(ordered derivative `R7F701374A`).

> **This repository _is_ the SIP.** Everything under `BSW/`, `Demo/`, `Doc/`, `BSWMD/`,
> `Generators/`, `DaVinciConfigurator/`, `MakeSupport/`, `Misc/` and `FlashTool/` comes from
> Vector delivery **CBD1800284 D00** unless a page is explicitly marked otherwise.

## Start here

- [Vector SIP overview](sip/) — delivery identity, license, what's included
- [Modules by layer](modules/) — per-module reference (purpose, origin, API, files)
- [General documents](general/) — release notes, delivery info, user manuals, application notes
- [How to build](demo/#how-to-build-the-demos) — Green Hills RH850 build via `m.bat` / Makefiles

## AUTOSAR layers in this repo

| Layer | Pages | Content |
|---|---|---|
| Application Software | [ASW](asw/) | No production ASW in SIP; see Demo apps |
| Complex Device Drivers | [CDD](cdd/) | FBL core, Boot Manager, Comm Wrapper, Updater, Flash driver |
| Services | [Services](services/) | BswM, NvM, Fee, CanTp, PduR, Det, Crc, SecMod, WrapNv, VStdLib |
| ECU Abstraction | [ECU Abstraction](ecu-abstraction/) | CanIf, MemIf |
| MCAL | [MCAL](mcal/) | Can driver; RH850 MCAL is third-party (not shipped) |
| Common | [Common](common/) | `_Common` headers, compiler/platform abstraction |
| Demos | [Demo](demo/) | DemoFbl, DemoBm, DemoKeys |
| Tools | [Tools](tools/) | DaVinci, generators, BSWMD, make support, HexView |

## Vector vs. custom — how to read the badges

| Badge | Meaning |
|---|---|
| ![Vector](https://img.shields.io/badge/Vector--provided-blue) | Unmodified Vector MICROSAR file (proprietary Vector license) |
| ![FCA](https://img.shields.io/badge/Vector--provided%2C%20FCA--customised-purple) | Vector file customised for the FCA program |
| ![Custom](https://img.shields.io/badge/Custom-green) | OEM/in-house integration code (MIT, demo templates) |
| ![Generated](https://img.shields.io/badge/Generated-yellow) | DaVinci/HexView generator output — do not edit by hand |
| ![Third-party](https://img.shields.io/badge/Third--party-red) | External component (e.g. Renesas MCAL), not delivered |

In-house documentation and site content is **MIT licensed** (see `LICENSE` at the repository root).
All `BSW/*` sources keep their Vector copyright headers and remain governed by the
Vector license terms (`SipLicense.lic`, `BetaDisclaimer.txt`).

## Repository map

```text
BSW/                  Vector MICROSAR BSW + FBL sources (21 modules)
BSWMD/                AUTOSAR module descriptions (.arxml)
Demo/                 DemoFbl + DemoBm applications, GenData, DemoKeys
Doc/                  Original Vector PDFs/HTML (sources of docs/general)
DaVinciConfigurator/  DaVinci Configurator installation (tooling)
Generators/           DaVinci generator schemes + BSWMD copies
MakeSupport/          Vector PES make environment (GHS/RH850)
Misc/                 HexView tool + FblUpd helpers
FlashTool/            Seed-key DLL + flash tool installer template
docs/                 This Astro Starlight site
.github/              Pages deployment + Dependabot automation
```
