# AutoCAD 2025 Shift-Ortho Fix

Fix for the AutoCAD 2025 Shift-Ortho issue commonly seen on HP laptops.

## Problem

On some HP laptops running AutoCAD 2025, `Left Shift` does not reliably toggle **Ortho Mode** as expected.

## What this fix does

This workaround runs at Windows logon and remaps `Left Shift` behavior for AutoCAD by sending `F8` when the key is pressed and released.

It only targets:

- `acad`
- `acadlt`

## Included files

```text
scripts/ACAD_ShiftOrtho.ps1
scripts/Launch_ACAD_ShiftOrtho.vbs
task-scheduler/ACAD_ShiftOrtho.xml
