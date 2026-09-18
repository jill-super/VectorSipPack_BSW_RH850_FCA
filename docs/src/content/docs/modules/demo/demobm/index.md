---
title: "DemoBm"
sidebar:
  order: 2
---

# DemoBm

![Custom](https://img.shields.io/badge/Custom-green) ![Layer](https://img.shields.io/badge/layer-demo-lightgrey)

> **Origin:** Custom (OEM integration). Boot-manager demo application in `Demo/DemoBm/Appl`.

## Purpose

Minimal Boot Manager program (`fbl_apbm.c/h`, `startup.c`) exercising `BSW/FblBm`: boot-condition checks
and jump-to-target logic. Companion to DemoFbl for the FCA startup flow.

## Build

```bat
cd Demo\DemoBm\Appl
m.bat
```

## Dependencies

`FblBm`, `Fbl`, `MakeSupport`
