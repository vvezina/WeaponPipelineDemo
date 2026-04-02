# UE5 Weapon Pipeline Tool

Editor tool built entirely in Blueprint to automate weapon asset creation, validation, and correction within a production pipeline. Built as a demo to showcase Blueprint-driven tooling in Unreal Engine 5.7.

## Tool Preview

![Weapon Pipeline Tool](Docs/tool_preview.png)

## Features

### Create Weapon
- Enter a weapon name to generate a new Data Asset from a template
- Automatically skips creation if an asset with that name already exists

### Validate Weapons
- Scans all weapon Data Assets and flags issues such as:
  - Missing Mesh, Niagara FX, or Sound references
  - Invalid values (Damage, Fire Rate, MaxAmmo <= 0)
- Outputs categorized log entries (Warning, Error, Skipped, Created, Fixed)

### Fix Invalid Weapons
- Auto-corrects invalid numeric values using class defaults
- Logs every change per asset so designers can review what was fixed

## Tech
- Unreal Engine 5.7
- 100% Blueprint — Editor Utility Widget, Data Assets, Enums
- No C++ or Python

