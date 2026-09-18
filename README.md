<p align="center">
  <img alt="Docs" src="https://img.shields.io/badge/docs-GitHub%20Pages-blue">
  <img alt="License" src="https://img.shields.io/badge/license-MIT-green">
  <img alt="Platform" src="https://img.shields.io/badge/platform-Renesas%20RH850-blue">
  <img alt="Language" src="https://img.shields.io/badge/language-C-orange">
  <img alt="AUTOSAR" src="https://img.shields.io/badge/AUTOSAR-Classic%20BSW-lightgrey">
  <img alt="SIP" src="https://img.shields.io/badge/SIP-CBD1800284-purple">
</p>

# BSW_RH850_FCA

Vector MICROSAR **Flash Bootloader Software Integration Package (SIP) CBD1800284**
for the **FCA SLP5** program (customer: Nexteer), targeting **Renesas RH850**
derivatives (ordered derivative `R7F701374A`). Secure boot / secure flashing demo
with bootloader, boot manager, updater, memory stack, CAN stack and crypto.

> 📚 **Full documentation site (GitHub Pages):** once Pages is enabled for this repo,
> the Astro Starlight site in [`docs/`](docs/) is published automatically by
> [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml).
> Start at [`docs/index.md`](docs/src/content/docs/index.md) → [Vector SIP](docs/src/content/docs/sip/) →
> [Modules by layer](docs/src/content/docs/modules/).

---

## Table of contents

- [What is in this repository?](#what-is-in-this-repository)
- [AUTOSAR layers](#autosar-layers)
- [Module inventory (layer + origin)](#module-inventory-layer--origin)
- [Vector vs. custom — how to read this repo](#vector-vs-custom--how-to-read-this-repo)
- [Installation & build](#installation--build)
- [Repository structure](#repository-structure)
- [Documentation](#documentation)
- [License](#license)
- [Contributing](#contributing)

---

## What is in this repository?

This repository **is the SIP in Git form**: Vector BSW sources, AUTOSAR module
descriptions, DaVinci configuration, demo bootloader/boot-manager applications,
build environment, flashing tools and the complete Vector document set —
plus a Markdown/Astro documentation layer ([`docs/`](docs/)) generated from it.

Key facts (from [`SipLicense.lic`](SipLicense.lic)):

| Field | Value |
|---|---|
| Delivery | `CBD1800284_D00` |
| SIP number | `20.07.00` |
| Customer / program | Nexteer / FBL FCA SLP5 |
| Ordered derivative | R7F701374A |
| Beta disclaimer | applies — see [`BetaDisclaimer.txt`](BetaDisclaimer.txt) |

---

## AUTOSAR layers

<details>
<summary><strong>Layer map (click to expand)</strong></summary>

| AUTOSAR layer | In this repo | Docs |
|---|---|---|
| Application Software (ASW) | No production ASW — behaviour shown by demos | [docs/asw/](docs/src/content/docs/asw/) |
| Complex Device Drivers (CDD) | FBL core, Boot Manager, Comm Wrapper, Updater, Flash driver, ASR stubs | [docs/cdd/](docs/src/content/docs/cdd/) |
| Services | BswM, NvM, Fee, CanTp, PduR, Det, Crc, SecMod, WrapNv, VStdLib | [docs/services/](docs/src/content/docs/services/) |
| ECU Abstraction | CanIf, MemIf | [docs/ecu-abstraction/](docs/src/content/docs/ecu-abstraction/) |
| MCAL | CAN driver; RH850 MCAL itself is third-party (not shipped) | [docs/mcal/](docs/src/content/docs/mcal/) |
| Common / infra | `_Common` headers, compiler/platform abstraction | [docs/common/](docs/src/content/docs/common/) |
| Demo | DemoFbl (CAN-FD, FCA SLP5), DemoBm, DemoKeys | [docs/demo/](docs/src/content/docs/demo/) |
| Tools | DaVinci, generators, BSWMD, make support, HexView, Flash tool | [docs/tools/](docs/src/content/docs/tools/) |

```text
            ┌──────────────────────────────────────────────┐
            │ Demo (DemoFbl / DemoBm)      [no prod. ASW]  │
            ├──────────────────────────────────────────────┤
            │ CDD: Fbl · FblBm · FblCw · FblUpd · Flash    │
            ├──────────────────────────────────────────────┤
            │ Services: BswM NvM Fee CanTp PduR Det Crc   │
            │           SecMod WrapNv VStdLib             │
            ├──────────────────────────────────────────────┤
            │ ECU Abstr.: CanIf · MemIf                   │
            ├──────────────────────────────────────────────┤
            │ MCAL: Can driver · (Renesas RH850 MCAL ext.) │
            └──────────────────────────────────────────────┘
```

</details>

---

## Module inventory (layer + origin)

<details>
<summary><strong>Full module table (click to expand)</strong></summary>

| Module | Path | AUTOSAR layer | Origin | Docs |
|---|---|---|---|---|
| Fbl | `BSW/Fbl` | CDD | Vector-provided, FCA-customised | [page](docs/src/content/docs/modules/cdd/fbl/) |
| FblBm | `BSW/FblBm` | CDD | Vector-provided | [page](docs/src/content/docs/modules/cdd/fblbm/) |
| FblCw | `BSW/FblCw` | CDD | Vector-provided, FCA-customised | [page](docs/src/content/docs/modules/cdd/fblcw/) |
| FblUpd | `BSW/FblUpd` | CDD | Vector-provided | [page](docs/src/content/docs/modules/cdd/fblupd/) |
| FblAsrStubs | `BSW/FblAsrStubs` | CDD | Vector-provided | [page](docs/src/content/docs/modules/cdd/fblasrstubs/) |
| Flash | `BSW/Flash` | CDD | Vector (+ generated ROM image) | [page](docs/src/content/docs/modules/cdd/flash/) |
| BswM | `BSW/BswM` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/bswm/) |
| NvM | `BSW/NvM` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/nvm/) |
| Fee_30_SmallSector | `BSW/Fee_30_SmallSector` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/fee_30_smallsector/) |
| CanTp | `BSW/CanTp` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/cantp/) |
| PduR | `BSW/PduR` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/pdur/) |
| Det | `BSW/Det` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/det/) |
| Crc | `BSW/Crc` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/crc/) |
| SecMod | `BSW/SecMod` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/secmod/) |
| WrapNv | `BSW/WrapNv` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/wrapnv/) |
| VStdLib | `BSW/VStdLib` | Services | Vector-provided | [page](docs/src/content/docs/modules/services/vstdlib/) |
| CanIf | `BSW/CanIf` | ECU Abstraction | Vector-provided | [page](docs/src/content/docs/modules/ecu-abstraction/canif/) |
| MemIf | `BSW/MemIf` | ECU Abstraction | Vector-provided | [page](docs/src/content/docs/modules/ecu-abstraction/memif/) |
| Can | `BSW/Can` | MCAL | Vector-provided | [page](docs/src/content/docs/modules/mcal/can/) |
| Mcal_Rh850P1xC | `BSW/Mcal_Rh850P1xC` | MCAL | Third-party (Renesas, not shipped) | [page](docs/src/content/docs/modules/mcal/mcal_rh850p1xc/) |
| _Common | `BSW/_Common` | Common | Vector-provided | [page](docs/src/content/docs/modules/common/shared-headers/) |
| DemoFbl | `Demo/DemoFbl` | Demo | Custom + Generated | [page](docs/src/content/docs/modules/demo/demofbl/) |
| DemoBm | `Demo/DemoBm` | Demo | Custom | [page](docs/src/content/docs/modules/demo/demobm/) |

SIP-mirrored pages (delivery scope, FCA customisation notes) live under
[`docs/sip/modules/`](docs/src/content/docs/sip/modules/) — e.g. [SIP: Det](docs/src/content/docs/sip/modules/services/det.md).

</details>

---

## Vector vs. custom — how to read this repo

| Badge | Meaning | License |
|---|---|---|
| ![Vector](https://img.shields.io/badge/Vector--provided-blue) | Unmodified Vector MICROSAR file | Proprietary Vector terms |
| ![FCA](https://img.shields.io/badge/Vector--provided%2C%20FCA--customised-purple) | Vector file customised for FCA | Proprietary Vector terms |
| ![Custom](https://img.shields.io/badge/Custom-green) | OEM/in-house integration (demo `fbl_ap*`, configs you write) | MIT |
| ![Generated](https://img.shields.io/badge/Generated-yellow) | DaVinci/HexView output (`GenData/`, `FlashRom.c`) — regenerate, don't hand-edit | Per generator |
| ![Third-party](https://img.shields.io/badge/Third--party-red) | External component (Renesas MCAL, JRE) — not delivered here | Vendor terms |

Every documentation page states its origin with one of these badges.
Assumption, stated explicitly: the whole tree is SIP CBD1800284, so anything
without a `Custom`/`Generated` marker is treated as Vector-provided.

---

## Installation & build

### Prerequisites

| Item | Requirement |
|---|---|
| Host | Windows (batch builds: `m.bat`, `b.bat`) |
| Toolchain | Green Hills (GHS) for RH850 |
| Hardware | Renesas RH850 (C1x / E1x family; ordered derivative R7F701374A) |
| Make env | `MakeSupport/cmd` GNU/Cygwin utilities on `PATH` |
| Config tool | Shipped `DaVinciConfigurator/` (see [Tools](docs/src/content/docs/tools/)) |
| Docs site (optional) | Node.js LTS + npm (`docs/package.json`) to preview the Astro site locally |

### Build the demos

```bat
cd Demo\DemoFbl\Appl
m.bat            :: builds the FBL demo (CAN-FD, FCA SLP5)

cd ..\..\DemoBm\Appl
m.bat            :: builds the Boot Manager demo
```

How it works: each `Appl/Makefile` pulls in `Makefile.config`,
`Makefile.derivative.*`, `Makefile.project.part.defines` on top of
`MakeSupport/Global.Makefile.target.make.3`, plus per-module fragments
`BSW/<Mod>/mak/*_{defs,cfg,rules,check}.mak`. Regenerate `GenData/` from
`Demo/DemoFbl/Config/` with DaVinci after any configuration change.

### CAN-wakeup wiring

See [`Demo/DemoFbl/Appl/README_CanWakeup.txt`](Demo/DemoFbl/Appl/README_CanWakeup.txt)
([rendered](docs/src/content/docs/general/can-wakeup-note.md)): RH850C1x → INTP2–5 on Port 0_5–0_8;
RH850E1x → IRQ0–3 on Port 2_0–2_3.

### Preview the docs site locally

```bash
cd docs
npm install
npm run dev
```

### ⚠️ Demo keys are not production keys

[`Demo/DemoKeys/`](Demo/DemoKeys) (`ccc_key_*`) are **demonstration only**.
Replace them with the OEM key-management flow (see [SecMod](docs/src/content/docs/modules/services/secmod/)).

---

## Repository structure

```text
BSW/                   Vector MICROSAR BSW + FBL sources (21 modules, each with mak/)
BSWMD/                 AUTOSAR module descriptions (.arxml, incl. EcuC + MCAL copies)
Demo/                  DemoFbl + DemoBm apps, DaVinci Config/, GenData/, DemoKeys/
Doc/                   Original Vector documents (PDF/HTML/CHM) — sources of docs/general
DaVinciConfigurator/   Configurator installation (tooling, third-party JRE)
Generators/            DaVinci generator schemes + BSWMD copies
MakeSupport/           Vector PES make environment (GHS/RH850)
Misc/                  HexView checksum/C-array tool + FblUpd helpers
FlashTool/             Seed-key DLL + flash-tool installer template
docs/                  Astro (Starlight) site: layers, modules, SIP, conversions
.github/               Pages deployment, Dependabot, auto-merge workflows
SipLicense.lic         SIP delivery identity (CBD1800284 D00)
BetaDisclaimer.txt     Vector beta disclaimer (liability exclusion)
LICENSE                MIT license (+ third-party notice)
```

---

## Documentation

- 🌐 **Site:** [`docs/`](docs/) (Starlight theme) — [overview](docs/src/content/docs/index.md)
- 📦 **SIP:** [Vector SIP CBD1800284](docs/src/content/docs/sip/) — delivery identity, content map, per-module SIP pages
- 🧩 **Modules:** [Modules by layer](docs/src/content/docs/modules/) — purpose, origin, key files, API excerpts, dependencies
- 📄 **Converted documents:** [General documents](docs/src/content/docs/general/) (release notes, delivery info,
  user manuals, application notes) + per-module Technical References linked from each module page
- 🗂️ **Originals:** [`Doc/`](Doc/) (authoritative PDFs/HTML), [`DocumentationGuide_VectorAUTOSAR.pdf`](DocumentationGuide_VectorAUTOSAR.pdf)

> Conversion note: PDFs were converted with text extraction into structured Markdown
> (headings, lists, key tables preserved). Complex layouts, figures and screenshots are
> summarised, not reproduced — each page links back to its source file, which remains
> authoritative. No `.doc/.docx` files were found in the repo (only `.pdf`, `.txt`, `.html`, `.chm`).

---

## License

In-house content in this repository is under the **[MIT License](LICENSE)**.
Third-party components — all Vector MICROSAR sources, tooling and documents, plus the
Renesas MCAL reference — keep their own license terms (see the
["Third-party components" section of LICENSE](LICENSE) and [`SipLicense.lic`](SipLicense.lic)).

---

## Contributing

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes
4. Push to your branch
5. Open a pull request — docs changes under `docs/` trigger the Pages preview build

*Docs generated from SIP CBD1800284 (September 2025 baseline). For issues, open a GitHub issue or PR.*
