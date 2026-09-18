---
title: "DemoFbl"
sidebar:
  order: 1
---

# DemoFbl

![Custom](https://img.shields.io/badge/Custom-green) ![Layer](https://img.shields.io/badge/layer-demo-lightgrey)

> **Origin:** Custom (OEM integration) + Generated (DaVinci/HexView). Application templates in
> `Appl/Source` and `Appl/Include` are Vector example code customised by the integrator (MIT for your changes);
> `Appl/GenData` is DaVinci-generated — never edit by hand, regenerate from `Config/`.

## Purpose

Complete FBL demo for FCA SLP5 (CAN-FD, `DemoFBL_CAN_FD_Fca_SLP5.dbc`, ECUC/System config in `Config/`).
Shows the full integration: startup (`startup.c`), application callbacks (`fbl_ap*.c`),
NV config (`WrapNv_Cfg.c`), seed/key hook (`Sec_SeedKeyVendor.c`), CAN-wakeup wiring.

## Key files

```text
Demo/DemoFbl/Appl/Source/fbl_ap.c|fbl_apdi.c|fbl_apnv.c|fbl_apwd.c|startup.c
Demo/DemoFbl/Appl/Source/Sec_SeedKeyVendor.c
Demo/DemoFbl/Appl/Include/fbl_ap.h|applfbl.h|comdat.h|MemMap.h|Compiler_Cfg.h
Demo/DemoFbl/Appl/GenData/*.c|*.h (+ include/, src/ for Fls)
Demo/DemoFbl/Config/** (DaVinci project: ECUC, System, ServiceComponents, user_config.cfg)
Demo/DemoFbl/Appl/Makefile* (+ m.bat/b.bat/j.bat)
Demo/DemoFbl/Appl/README_CanWakeup.txt
```

## Build

```bat
cd Demo\DemoFbl\Appl
m.bat
```

## Dependencies

`Fbl`, `FblCw`, `Can`, `CanIf`, `CanTp`, `PduR`, `NvM`, `Fee_30_SmallSector`, `SecMod`, `WrapNv`, `Flash`

## See also

- [CAN wakeup note](../../../general/can-wakeup-note/) · [Startup manual](../../../general/startup-fca-slp5/) · [Fbl](../../cdd/fbl/)
