---
title: "Basic Software – MCAL"
sidebar:
  order: 50
---

# Basic Software – MCAL

Microcontroller Abstraction Layer: MCU-specific drivers (CAN driver, RH850 MCAL hooks). The Renesas RH850 MCAL itself is third-party and not part of this delivery.

## Modules

- [Can](../modules/mcal/can/) — MICROSAR CAN driver (MCAL)
- [Mcal_Rh850P1xC](../modules/mcal/mcal_rh850p1xc/) — Renesas MCAL integration point (third-party, not shipped)

## Third-party note

The RH850 MCAL itself comes from Renesas. Read the [3rd-party MCAL integration](../modules/mcal/mcal_rh850p1xc/#converted-vector-documents) references before integrating.
