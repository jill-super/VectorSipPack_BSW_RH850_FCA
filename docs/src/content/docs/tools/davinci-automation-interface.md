---
title: "DaVinci Configurator Automation Interface"
---

# DaVinci Configurator Automation Interface

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Third-party](https://img.shields.io/badge/Third--party-red) ![Category](https://img.shields.io/badge/category-Tools-lightgrey)

> **Source:** `DaVinciConfigurator/Core/AutomationInterface/_doc/DVCfg_AutomationInterfaceDocumentation.pdf` (3.4 MB; companion `DVCfg_AutomationInterface_Javadoc.zip` and `templates/` in the same folder). The original PDF is authoritative; this page is a structured summary because the document is third-party tooling material shipped inside the `DaVinciConfigurator/` installation, not part of the `Doc/` SIP document set. Text extraction preserves headings and key points; API details, diagrams and Javadoc remain in the originals.

## What this document covers

Automation interface of DaVinci Configurator: how to drive the configurator headlessly / from scripts (project creation, input-file handling, validation, code generation) instead of the GUI. Companions the Javadoc ZIP (Java API reference) and the `templates/` example scripts in the same `_doc` folder.

## When you need it

- Regenerating `Demo/DemoFbl/Appl/GenData/` after changing `Demo/DemoFbl/Config/` without clicking through DaVinci.
- CI / batch configuration flows built on the shipped `DaVinciConfigurator/` installation.
- Writing Groovy/Java automation against the Configurator API (see the Javadoc ZIP).

## Outline (from file context)

- Installation location: `DaVinciConfigurator/Core/AutomationInterface/_doc/`
- Main PDF: `DVCfg_AutomationInterfaceDocumentation.pdf` — concepts, setup, API walkthrough, examples.
- API reference: `DVCfg_AutomationInterface_Javadoc.zip` — generated Javadoc, open in a browser after unzipping.
- Templates: `_doc/templates/` — starter scripts referenced by the PDF.

## How to use

1. Keep using the GUI path in [Startup FCA SLP5](../general/startup-fca-slp5/) for first-time setup.
2. For scripting, read the PDF's getting-started + example sections, then adapt a `templates/` script to point at `Demo/DemoFbl/DemoFbl.dpa` / `Demo/DemoFbl/Config/`.
3. Regenerate `GenData/` with DaVinci after any configuration change; never hand-edit generated files.

## License note

`DaVinciConfigurator/` including this document is third-party Vector tooling governed by its own license terms (see the `licenses/` folder next to the binaries), not by the repository's MIT license for in-house documentation content.

## See also

- [Tools and Configuration](./) — `DaVinciConfigurator/`, `Generators/`, `BSWMD/`, `MakeSupport/`, HexView, Flash tool.
- [DemoFbl](../modules/demo/demofbl/) — the demo project this automation regenerates.
- [DaVinci licenses](./technicalreference-davinciconfigurator-licenses/) — license handling reference.
