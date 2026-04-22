---
title: CSV Processing Info
type: outcome
created: 2026-04-22
updated: 2026-04-22
sources: [CSV_Processing_Info.md]
tags: [outcomes]
---

Outcome that provides information about failures in a .CSV file for a mesh workflow step, automatically added upon completion.

## Overview

**CSV Processing Info** reports on issues encountered while processing a .CSV file during a mesh workflow operation. It is automatically added and cannot be added manually.

## Details View

### General

| Field | Description |
|---|---|
| **Outcome Type** | Displays the selected outcome type |

### Definition

| Field | Description |
|---|---|
| **Lines Skipped** | Displays the skipped lines in the .csv file |
| **Failure Lines** | Displays the failed line numbers in the .csv file that caused the operation to fail or produce warnings |

## Steps That Produce This Outcome

- Automatically added to operations that process .CSV files; cannot be inserted manually

## Related Pages

- [[scope]]
- [[failure-info]]
- [[warning-info]]
