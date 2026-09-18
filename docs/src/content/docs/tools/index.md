---
title: "Tools and Configuration"
sidebar:
  order: 80
---

# Tools and Configuration

Configuration and build tooling: DaVinci Configurator data, generators, BSWMD, make support, HexView, Flash tool.

## Components

- **DaVinciConfigurator/** — DaVinci Configurator installation used to edit `Demo/DemoFbl/Config` and regenerate `GenData`.
- **Generators/Components/_Schemes/** — DaVinci generator schemes + BSWMD copies per module.
- **BSWMD/** — AUTOSAR basic-software module descriptions (`.arxml`) for every module incl. EcuC and MCAL copies.
- **MakeSupport/** — Vector PES make environment (`Global.Makefile.target.make.3`, GNU/Cygwin `cmd/` tools).
- **Misc/HexView/** — HexView checksum/C-array tool; see the [HexView reference](../general/reference-manual-hexview/).
- **FlashTool/** — `seedkey.dll`/template installer for the vFlash programming flow.

## Converted tool documents

- [DaVinci Configurator Automation Interface](./davinci-automation-interface/) — scripting/headless use of DaVinci (`DaVinciConfigurator/.../_doc/DVCfg_AutomationInterfaceDocumentation.pdf` + Javadoc).
- [DaVinci Configurator Licenses](./technicalreference-davinciconfigurator-licenses/)
- [LegacyDb2SystemDescr Converter](./technicalreference-gentool-csasrlegacydb2systemdescr-vector/)
