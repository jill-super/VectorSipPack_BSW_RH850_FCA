---
title: "Complex Device Drivers (CDD)"
sidebar:
  order: 20
---

# Complex Device Drivers (CDD)

Complex device drivers and bootloader components: Flash Bootloader (FBL), Boot Manager, Communication Wrapper, Updater and Flash driver.

## Modules

- [Fbl](../modules/cdd/fbl/) — Vector Flash Bootloader core (FBL FCA variant for SLP5): startup, memory programming, UDS diagnostics (fbl_diag_core + OEM diagnostics), flash interaction (fbl_mem, fbl_flio), watchdog handling and application validation/boot.
- [FblBm](../modules/cdd/fblbm/) — FBL Boot Manager: decides at reset whether to stay in the bootloader or jump to the application (boot conditions, target handling).
- [FblCw](../modules/cdd/fblcw/) — FBL Communication Wrapper: thin CAN-oriented communication layer (fbl_cw) connecting the bootloader diagnostics to CanIf/PduR/CanTp, FCA-customised (FblCw_Fca).
- [FblUpd](../modules/cdd/fblupd/) — FBL Updater (programming-session updater): minimal self-update component (upd_main) that reprograms the bootloader itself via templates in _Template.
- [FblAsrStubs](../modules/cdd/fblasrstubs/) — Bootloader-environment stubs for AUTOSAR modules absent in the FBL context (EcuM, ComM, Dem, Os/Rte, SchM).
- [Flash](../modules/cdd/flash/) — RH850 flash programming support: flashdrv (Vector flash driver for RH850/RV40) plus generated FlashRom C-array (HexView output) and GHS build files in Build/.
