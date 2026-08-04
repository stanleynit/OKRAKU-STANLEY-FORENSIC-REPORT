# README

## Digital Forensic Examination Report – `cartel.img`

### Overview

This repository contains a **Digital Forensic Examination Report** documenting the forensic analysis of the disk image **`cartel.img`**. The examination was performed as part of a **Digital Forensics and Incident Response** module using accepted forensic methodologies to preserve evidence integrity and recover potential digital artefacts.

### Report Information

* **Case Reference:** CARTEL-USB-2026-08
* **Examiner:** Stanley Gibson Okraku
* **Evidence:** `cartel.img`
* **Report Date:** 3 August 2026

### Objectives

The examination aimed to:

* Verify the integrity of the forensic image.
* Identify the file system and disk structure.
* Recover allocated and deleted files.
* Detect evidence of data wiping or destruction.
* Reconstruct a timeline of user activity.
* Document findings in accordance with forensic best practices.

### Tools Used

* SIFT Workstation
* The Sleuth Kit (`fls`, `icat`, `istat`, `mmls`, `img_stat`, `fsstat`)
* Foremost
* PhotoRec 7.1
* Linux Terminal Utilities
* LibreOffice Writer

### Examination Summary

The investigation confirmed that:

* The forensic image maintained integrity throughout the examination using MD5 and SHA-256 hash verification.
* The storage device is an unpartitioned FAT16 USB flash drive (~247.5 MB).
* Only two allocated files (gumbo recipe text files) remained visible.
* More than 80% of the disk had been deliberately overwritten with repeating **"SORRY"** and **"CHARLIE"** patterns, indicating intentional data destruction.
* Nine deleted files, including JPEG and GIF images and a text fragment, were successfully recovered through file carving.
* A recovered diary fragment referenced wiping a hard drive and reformatting the USB device.
* Duplicate JPEG files were identified using SHA-256 hash comparison.
* No direct evidence linking the device to cartel or drug-trafficking activity was recovered.

### Report Contents

The report includes:

1. Executive Summary
2. Evidence Integrity Verification
3. Initial Triage
4. Evidence Discovery Analysis
5. Deleted Data Recovery
6. Timeline Reconstruction
7. Conclusions
8. Recommendations
9. Supporting Command Outputs

### Key Findings

* Evidence integrity preserved through matching MD5 and SHA-256 hashes.
* FAT16 filesystem with no partition table.
* Large-scale intentional overwrite of the storage medium.
* Recovery of deleted multimedia files.
* Recovery of a diary fragment suggesting intentional destruction of previous data.
* Timeline reconstruction based on available metadata and recovered artefacts.

### Notes

This report presents factual forensic observations only. It does **not** determine legal guilt or innocence. Any legal interpretation should be made by the appropriate investigative or judicial authority.

### Author

**Stanley Gibson Okraku**
Digital Forensics and Incident Response
August 2026
