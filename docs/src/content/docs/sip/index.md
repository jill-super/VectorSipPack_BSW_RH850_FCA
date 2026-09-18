---
title: "Vector SIP (CBD1800284)"
sidebar:
  order: 100
---

# Vector SIP (CBD1800284)

![SIP](https://img.shields.io/badge/SIP-CBD1800284-purple)
![Customer](https://img.shields.io/badge/customer-Nexteer-lightgrey)
![Program](https://img.shields.io/badge/program-FBL%20FCA%20SLP5-blue)
![Derivative](https://img.shields.io/badge/derivative-R7F701374A-orange)

## What is the SIP?

The **Software Integration Package** is Vector's delivery unit for MICROSAR BSW:
sources (`BSW/`), module descriptions (`BSWMD/`), generator schemes (`Generators/`),
demo integration (`Demo/`), tooling (`DaVinciConfigurator/`, `MakeSupport/`, `Misc/`, `FlashTool/`)
and the document set (`Doc/`). **This repository is SIP CBD1800284 D00 in Git form.**

Delivery identity comes from `SipLicense.lic` at the repository root:

| Field | Value |
|---|---|
| Delivery | `CBD1800284_D00` |
| SIP number | `20.07.00` |
| Customer | Nexteer Automotive Corporation |
| Program | FBL FCA SLP5 |
| Ordered derivative | R7F701374A |
| Beta disclaimer | shown (`BetaDisclaimer.txt` applies) |

## License reality

- The SIP's **code** is proprietary Vector software (see each file's copyright header,
  `BetaDisclaimer.txt`, and the license parameters in `SipLicense.lic`).
            - This repo additionally uses the **MIT license** for in-house documentation/site content
              (see `LICENSE` at the repository root); it does **not** relicense Vector files.
- Always check the [Delivery readme](../general/readme-cbd1800284/) and the LUA/Product Information
  before redistributing anything.

## SIP content map

| SIP area | Repo path | Docs |
|---|---|---|
| BSW sources | `BSW/` | [Modules by layer](../modules/) |
| Demo integration | `Demo/` | [DemoFbl](../modules/demo/demofbl/), [DemoBm](../modules/demo/demobm/) |
| Module descriptions | `BSWMD/` | per-module BSWMD sections |
| Generators | `Generators/` | [Tools](../tools/) |
| Configurator | `DaVinciConfigurator/` | [Tools](../tools/) |
| Build env | `MakeSupport/` | [Tools](../tools/), [Demo build](../demo/#how-to-build-the-demos) |
| Documents | `Doc/` | [General documents](../general/) |
| Delivery meta | `SipLicense.lic`, `Doc/DeliveryInformation` | [Delivery pages](../general/#delivery-information) |

## Module pages (SIP view)

Per-module SIP pages live under `docs/sip/modules/<layer>/<module>.md` and mirror the
canonical [Modules by layer](../modules/) reference with SIP-specific notes
(delivery scope, FCA customisation, generation). Start from any layer:

- [CDD](../cdd/) · [Services](../services/) · [ECU Abstraction](../ecu-abstraction/)
- [MCAL](../mcal/) · [Common](../common/) · [Demo](../demo/) · [Tools](../tools/)

## Key SIP documents

- [Release Note FCA SLP5](../general/release-note-fca-slp5/)
- [Readme CBD1800284](../general/readme-cbd1800284/)
- [Issue Report CBD1800284](../general/issue-report-cbd1800284/)
- [Startup FCA SLP5](../general/startup-fca-slp5/)
- [User Manual Flash Bootloader](../general/user-manual-flash-bootloader/)
