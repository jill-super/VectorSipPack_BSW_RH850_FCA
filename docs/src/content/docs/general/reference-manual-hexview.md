---
title: "Reference Manual HexView"
sidebar:
  order: 1
---

# Reference Manual HexView

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Category](https://img.shields.io/badge/category-Tools-lightgrey)

> **Source:** `Misc/HexView/ReferenceManual_HexView.pdf` — 127 pages. The original file is authoritative; this page is a structured Markdown conversion (headings, lists and key points preserved; complex tables/figures/screenshots are summarised, not reproduced pixel-faithfully).

**Original metadata:** title `HexView` · author `Armin Happel`

## What this document covers

Reference manual for the HexView tool (Misc/HexView/hexview.exe): checksum calculation, C-array generation (FlashRom), expdatproc plug-ins.

## Document outline (extracted headings)

- Reference Manual HexView
- HexView
- Reference Manual
- Caution
- Authors Armin Happel
- Status Released
- Document Information
- History
- Author Date Version Remarks
- 70. Removed them as application modules.
- CBC in the parameter
- HEX-file
- Help menu
- NOAR-fields

## Key content (extracted text sample)

Reference Manual HexView 
© 2018 Vector Informatik GmbH Version 1.12.02 1 
based on template version 5.1.0 
 
 
 
 
 
 
 
 
 
 
 
HexView 
Reference Manual 
 
 
Version 1.12.02 
 
 
 
 
 
 
 
 
Caution 
Vector Informatik GmbH is furnishing this item “as is” and free of charge. Vector 
Informatik GmbH does not provide any warranty of the item whatsoever, 
whether express, implied, or statutory, including, but not limited to, any warranty 
of merchantability or fitness for a particular purpose or any warranty that the 
contents of the item will be error-free. 
 
 
 
Authors Armin Happel 
Status Released 
 
 

Reference Manual HexView 
© 2018 Vector Informatik GmbH Version 1.12.02 2 
based on template version 5.1.0 
Document Information 
History 
Author Date Version Remarks 
Vishp 2018-05-10 1.12.02 > Fiat container files not generated correctly 
> Neg. Hex-values not accepted 
> Public key hash overwritten when merging 
VBF 
> Sw_signature may written with no contents. 
Vishp 2018-02-13 1.12.01 > Fill operation with random data failed 
> Improve handling of LoadAddress for s-rec. 
Vishp 2018-02-05 1.12.00 > Fix range operation issues in V1.11 if not 
starting on block start address. 
> Fix checksum calculation issues of V1.11 for 
restricted ranges or checksum target 
address is located inside the csum data. 
> Remove BAFA restrictions to crypto 
operations. 
> Restricting compression/decompression to 
non-streaming operations. 
> Fixing verification_structure_address output 
for Ford-VBF V3.1. 
> Fix startup issue on some Windows10 PCs 
> Improved Hexview return codes 
Vishp 2017-08-03 1.11.01 > Performance improvements for large files 
operation (compared to 1.11.00). 
> Fix VBF generation issue. 
> Substitute binaries for VBF without changing 
the VBF header (/xvbfsubst). 
Vishp 2017-06-09 1.11.00 > Switches /gmal and /gmad for separate GM 
header alignment operations 
> Support for further VCC VBF version. 
> Support for further Ford VBF version. 
> Support for ed25519 signature 
> Remove encryption from standard package 
due to BAFA export restrictions. 
> Support for GM compression (0302) and 
BDL (0601) envelope types. 
> Support for signature verification 
> Support large files (see release notes). 
Vishp 2017-03-09 1.10.04 > Tag length calculation for validation structure 
corrected. 
> GM SLP5: Extend use of of cal-files from 20 
Reference Manual HexView 
© 2018 Vector Informatik GmbH Version 1.12.02 3 
based on template version 5.1.0 
to 128. 
> Extend number of regions from 32 to 256. 
> Extend number of partitions from 20 to 128. 
> Allow usage of CAL module IDs from 51 to 
70. Removed them as application modules. 
Vishp 2016-09-05 1.10.01 > Fixing dialog problem with HEX ASCII export 
> Allow long lines for HEX ASCII exports 
> Introduce /CSR for reverse csum output 
> Multiple modules for GM SLP4 export 
> DataTypes can be specified for GM cmpr. 
Sign. (envelope 3) 
> Value input with leading 0 no longer leads to 
interpretation of octal values. 
Vishp 2016-03-18 1.10.00 > MISRA and strict ANSI for C-File generation 
improved. 
> Extensions to expdatproc (RSA-PSS, RSA-
OAEP) 
> Hexview returned error codes even if no 
error was detected. 
> Checksum calculation over holes revised. 
> Support PKCS#1, PKCS#8 and X.509 
certificates as file input for RSA operations 
(without passwords). 
Vishp 2016-01-21 1.09.04 > Correcting data processing operations. 
Vishp 2015-08-28 1.09.03 > Allow sw_version in VBF V2.5 with no char. 
> […]

## How to use this document

- Integrators: read the linked sections before changing configuration or flashing.
- Keep the original PDF/HTML under version control; regenerate this page if the source changes.
