---
title: "Converted: Security Module (SecMod)"
sidebar:
  order: 2
---

# Converted: Technical Reference — Security Module (SecMod)

![Converted](https://img.shields.io/badge/converted--from-Vector%20PDF-yellow) ![Vector](https://img.shields.io/badge/origin-Vector--provided-blue)

> **Source:** `Doc/TechnicalReferences/TechnicalReference_SecurityModule.pdf` — 59 pages · original title `Security Module `. The PDF is authoritative; this conversion preserves structure and key statements, not print layout/figures.

## What this document covers

Vector Technical Reference for **Security Module (SecMod)**: feature description, configuration parameters, API tables, call sequences, constraints and integration notes for the MICROSAR module.

## Document outline (extracted headings)

- Security Module
- Technical Reference
- Authors Markus Schneider
- Status Released
- Technical Reference Security Module
- Document Information
- History
- Author Date Version Remarks
- Reference Documents
- Scope of the Document
- Contents
- 5.1.2 Create a checksum / signature file with HexView ............................. 19
- 5.1.3 Create an AES128 Encrypted file with HexView ...............................  19
- 5.2.2.1 Security class C ................................ ............................. 21

## Key content (extracted text sample)

Security Module 
Technical Reference 
 
 
Version 2.2.0 
 
 
 
 
 
 
 
 
 
 
 
Authors Markus Schneider 
Status Released 
 
Technical Reference Security Module 
© 2016 Vector Informatik GmbH Version 2.2.0 2 
based on template version 5.6.0 
Document Information 
History 
Author Date Version Remarks 
Christian Bäuerle 2010-10-13 1.0.4 Generalized technical reference 
Christian Bäuerle 2012-07-02 1.0.5 Minor corrections 
Markus Schneider 2013-11-27 2.0.0 Major rework 
Markus Schneider 2014-03-13 2.1.0 Rework of ‘Functional Description’; added 
additional informations; minor corrections 
André Caspari 2016-08-02 2.2.0 Updated API description 
Reference Documents 
No. Source Title Version 
[1] HIS API IO Library 2.0.3 
[2] HIS Security Module Specification 1.1 
[3] Vector HexView Reference Manual 1.6 
[4] RSA PKCS #1: RSA Cryptography Standard 2.1 
[5] IETF HMAC: Keyed-Hashing for Message Authentication RFC2104 Feb 1997 
[6] ANSI Keyed Hash Message Authentication Code X9.71 2000 
Scope of the Document 
This technical reference describes the general use of the Security Module software. 
 
Technical Reference Security Module 
© 2016 Vector Informatik GmbH Version 2.2.0 3 
based on template version 5.6.0 
Contents 
1 Introduction................................ ................................ ................................ ................... 8 
2 Software Architecture ................................ ................................ ................................ ... 9 
2.1 Security Module Components ................................ ................................ ............ 9 
3 Integration ................................ ................................ ................................ ................... 10 
3.1 Scope of Delivery ................................ ................................ ............................. 10 
3.2 Include Structure ................................ ................................ .............................. 10 
3.3 Compiler Abstraction and Memory Mapping ................................ ..................... 10 
4 Configuration ................................ ................................ ................................ .............. 11 
4.1 GENy ................................ ................................ ................................ ............... 11 
4.2 Security Module Configuration ................................ ................................ ......... 11 
4.3 Configuration Parameters ................................ ................................ ................ 11 
4.4 Key Files ................................ ................................ ................................ .......... 13 
4.4.1 Authenticity file mode ................................ ................................ ....... 14 
4.4.2 INI-Key file mode ................................ ................................ ............. 16 
4.5 Running the Generator ................................ ................................ .................... 17 
5 Preparation of the Application ................................ ................................ ................... 18 
5.1 HexView................................ ................................ ................................ ........... 19 
5.1.1 Fill and align the hex file with HexView ................................ ............. 19 
5.1.2 Create a checksum / signature file with HexView ............................. 19 
5.1.3 Create an AES128 Encrypted file with HexView ............................... 19 
5.2 Signature Generation ................................ ................................ ....................... 20 
5.2.1 Hash calculation ................................ ................................ ............... 20 
5.2.2 Signing operation ................................ ................................ ............. 21 
5.2.2.1 Security class C ................................ ............................. 21 
5.2.2.2 Security class CCC ................................ ........................ 23 
5.3 MkPsKeys ................................ ................................ ................................ ........ 25 
6 Functional Description ................................ ................................ ............................... 27 
6.1 Verification Module ................................ ................................ ........................... 27 
6.1.1 Variants […]

## Related module

See [SecMod](../) for purpose, API, files and dependencies.
