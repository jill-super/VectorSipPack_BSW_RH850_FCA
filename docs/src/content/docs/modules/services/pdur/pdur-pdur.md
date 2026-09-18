---
title: "Converted: PduR"
sidebar:
  order: 2
---

# Converted: Technical Reference — PduR

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_PduR.pdf` — 71 pages · original title `MICROSAR PDU Router`. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **PduR**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- MICROSAR PDU Router
- Technical Reference
- DaVinci Configurator
- Status Released
- Technical Reference MICROSAR PDU Router
- Document Information
- History
- Author Date Version Remarks
- Reference
- IF Gateway
- ESCAN00064126
- Loadable
- Added Cancel- Receive/ Transmit Support
- TxConfirmation and RxIndication according

## Key content (extracted text sample)

MICROSAR PDU Router 
Technical Reference 
 
DaVinci Configurator 
Version 3.04.00 
 
 
 
 
 
 
 
 
 
 
 
Authors Erich Schondelmaier, Gunnar Meiss, Sebastian 
Waldvogel, Florian Röhm, Büsra Bayrak, Heiko Hübler 
Status Released 
 
 
 
 
 
Technical Reference MICROSAR PDU Router 
© 2018 Vector Informatik GmbH Version 3.04.00 2 
based on template version 4.9.2 
Document Information 
History 
Author Date Version Remarks 
Erich Schondelmaier 2012-12-20 1.00.00 Initial version based on PduR Technical 
Reference 
Erich Schondelmaier 2012-07-12 2.00.00 Adapted to AUTOSAR 4.0.3 
Erich Schondelmaier 2012-10-15 2.01.00 TP Gateway 
IF Gateway 
Gunnar Meiss 2012-11-21 2.02.00 AR4-285: Support PduRRoutingPathGroups 
Erich Schondelmaier 2013-02-07 2.02.01 Adapted Tp- API description 
Erich Schondelmaier 2013-02-15 2.02.02 Added some ASR deviations 
ESCAN00064126 
Erich Schondelmaier 2013-03-19 2.03.00 ESCAN00064364 AR4-325: Post-Build 
Loadable 
Added Cancel- Receive/ Transmit Support 
Erich Schondelmaier 2014-04-15 2.04.00 Added TP routing with variable addresses 
(MetaData Handling) 
Added Threshold “0” support 
Erich Schondelmaier 2014-04-15 2.04.01 Support the StartOfReception API (with the 
PduInfoType), 
TxConfirmation and RxIndication according 
ASR4.1.2 
Erich Schondelmaier 2014-09-01 2.05.00 Added SecOC to the Interface Overview 
Extended Tp Gateway Routing behavior 
description 
Updated Configuration Variant 
Sebastian Waldvogel 2015-02-23 2.06.00 FEAT-1057: Added documentation about 
configuration of range rou ting paths and 
functional requests gateway 
Sebastian Waldvogel 2015-05-11 2.06.01 FEAT-1057: Improvements of documentation 
Florian Röhm 2015-07-30 2.07.00 FEAT-109: Added documentation for PduR 
switching feature and N:1 routing paths 
Florian Röhm 2016-01-16 2.08.00 FEAT-1485: Added documentation for 1:N 
and N:1 transport protocol routing paths 
Gunnar Meiss 2016-02-25 2.08.00 FEAT-1631: Trigger Transmit API with 
SduLength In/Out according to ASR4.2.2 
Erich Schondelmaier 2016-03-17 2.08.00 added limitation: 
- The Polling Mode cannot be used for N:1 
routings. 
- Cancel Transmit for N:1 routing paths is 
only supported if a Tx Confirmation is 
enabled. 
- Removed limitation: N:1 interface routing 
paths suppport only for lower layer CanIf. 
Technical Reference MICROSAR PDU Router 
© 2018 Vector Informatik GmbH Version 3.04.00 3 
based on template version 4.9.2 
Florian Röhm 2016-04-01 2.08.01 Removed empty chapters 
Erich Schondelmaier, 
Florian Röhm 
2016-08-10 3.00.00 Shared/Dedicated Buffer support 
Memory mapping extension 
Sebastian Waldvogel 2016-11-24 3.00.00 Smart Learning (Switching) 
Florian Röhm 2017-06-22 3.00.01 ESCAN00095254: Missing DET error 
PDUR_E_PDU_INSTANCES_LOST 
description in case of N:1 communication 
interface routings with upper layer 
Florian Röhm 2017-06-23 3.00.01 STORYC-1629: N:1 routing path support for 
IpduM Container feature 
Florian Röhm 2017-09-21 3.01.00 STORYC-1972: Support 1:N Tx IF API 
Forwarding 
Büsra Bayrak 2017-11-07 3.02.00 STORYC-2031: Support buffered IF API 
Forwarding routing paths 
Florian Röhm 2018-01-30 3.03.00 STORYC-3416: PduR: Enable assignment of 
buffers smaller than the associated PDU 
sizes to the buffer po ol referenced by a 
routing path 
STORYC-3435: PduR: Enable routing paths 
with different connected PDU sizes in 
gateway routings 
Heiko Hübler 2018-03-07 3.04.00 Maintenance (STORYC-3934) 
Technical Reference MICROSAR PDU Router 
© 2018 Vector Informatik GmbH Version 3.04.00 4 
based on template version 4.9.2 
Reference Documents 
No. Source Title Version 
[1] AUTOSAR AUTOSAR_SWS_PDURouter.pdf 4.0.3 
[2] AUTOSAR AUTOSAR_SWS_PDURouter.pdf. 4.1.1 
[3] AUTOSAR AUTOSAR_SWS_PDURouter.pdf 4.1.2 
[4] AUTOSAR AUTOSAR_SWS_DevelopmentErrorTracer.pdf 3.2.0 
[5] AUTOSAR AUTOSAR_TR_BSWModuleList.pdf 1.6.0 
[6] AUTOSAR AUTOSAR_SWS_SAEJ1939TransportLayer.pdf 1.5.0 
[7] Vector TechnicalReference_CanIf.pdf 6.02.00 
[8] Vector TechnicalReference_<CAN Driver>.pdf - 
[9] AUTOSAR TechnicalReference_CanTp.pdf 2.00.00 
 
This technical reference describes the general use of the PduR basis software module. 
 
 
 
 
Caution 
We have configured the programs in accordance with your specifications in the 
questionnaire. Whereas the programs do support other configurations than the one 
specified in your questionnaire, Vector´s release of the programs delivered to your 
company is expressly restricted to the configuration you have specified in the 
questionnaire. 
 
 […]

## Related module

See [PduR](../) for purpose, API, files and dependencies.
