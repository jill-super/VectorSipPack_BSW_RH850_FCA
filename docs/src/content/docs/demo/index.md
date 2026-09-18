---
title: "Demo Applications"
sidebar:
  order: 70
---

# Demo Applications

Demonstration bootloader/boot-manager applications and OEM integration templates.

## Applications

- [DemoFbl](../modules/demo/demofbl/) — full flash-bootloader demo (CAN-FD, FCA SLP5 config)
- [DemoBm](../modules/demo/demobm/) — boot-manager demo

## How to build the demos

Requirements: Green Hills (GHS) RH850 toolchain, Windows host with `MakeSupport/cmd` utilities on `PATH`.

```bat
cd Demo\DemoFbl\Appl
m.bat            :: build the FBL demo
cd ..\..\DemoBm\Appl
m.bat            :: build the Boot Manager demo
```

The build is driven by the per-project `Makefile` (includes `Makefile.config`,
`Makefile.derivative.*`, `Makefile.project.part.defines`) on top of
`MakeSupport/Global.Makefile.target.make.3`, plus the per-module
`BSW/<Mod>/mak/*_defs.mak|*_cfg.mak|*_rules.mak|*_check.mak` fragments.

CAN-wakeup port setup is documented in
`Demo/DemoFbl/Appl/README_CanWakeup.txt`:
RH850C1x uses INTP2–5 on Port 0_5–0_8; RH850E1x uses IRQ0–3 on Port 2_0–2_3.

## DemoKeys

`Demo/DemoKeys/` holds **demonstration only** crypto keys (`ccc_key_*`).
Never use them in production; replace with the OEM key-management flow
(see [SecMod](../modules/services/secmod/)).
