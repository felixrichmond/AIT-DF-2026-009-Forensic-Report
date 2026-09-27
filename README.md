# Case ID: AIT-DF-2026-009 — Digital Forensic Investigation Report

**Organization:** Apex Integrated Technologies Ltd. — DFIR Unit  
**Investigator:** Felix Richmond
**Date:** September 27, 2026  
**Status:** Completed & Submitted  

---

## Executive Overview

This repository contains the official **Digital Forensic Investigation Report** for **Case ID: AIT-DF-2026-009**. The inquiry was conducted to analyze, verify, and reconstruct deleted directory structures and graphic design assets from an enterprise workstation disk image (`Evidence.E01`).

The investigation adhered strictly to **ISO/IEC 27037 standards** for digital evidence handling and employed a validated multi-tool methodology incorporating `dd`, `R-Drive Image`, `FTK Imager (v8.3.0.27)`, and `Autopsy (v4.23.1)`.

---

## Key Investigation Highlights

* **Cryptographic Evidence Verification:** The evidence image `Evidence.E01` was verified pre- and post-analysis maintaining complete bit-for-bit cryptographic integrity:
  * **SHA-256:** `6216149FDDF6EB7074349AFAEF226F02C3B246EE6C3C3AE91C5AB7ADEB8C29E0`
  * **MD5:** `ae39e9a30ab5a65809eb93289938e149`
* **Deletion Status & Recovery:** 
  * Target directories `SSH`, `Corel`, and `corel draw work` were confirmed deleted within the active `$MFT` root index.
  * Directories `My pic`, `Our pic`, and `ADDS Project` were unallocated from parent directory records, requiring sector carving.
  * Autopsy successfully parsed **1,162 deleted file records** and recovered primary project files (including Corel PHOTO-PAINT `.cpt` graphic assets).
* **Defensible Deletion Window:** Forensic timeline reconstruction established the primary deletion event between **September 16, 2026, 11:01:30 WAT** and **September 24, 2026, 11:42:43 WAT**.

---

## Deliverables in This Repository

| File Name | Description |
| :--- | :--- |
| **`Forensic_Investigation_Report.pdf`** | Primary comprehensive investigation report covering evidence verification, folder analysis, forensic screenshots, timeline reconstruction, and cross-tool validation matrices. |

---

## Direct Links & Submission Reference

* **Repository URL:** `https://github.com/your-username/AIT-DF-2026-009-Forensic-Report`
* **Direct Report PDF:** `https://github.com/your-username/AIT-DF-2026-009-Forensic-Report/blob/main/Forensic_Investigation_Report.pdf`

---
*Prepared for Apex Integrated Technologies Ltd. Digital Forensics & Incident Response Division.*
