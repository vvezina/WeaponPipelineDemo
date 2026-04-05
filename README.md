# Weapon Asset Validator

Editor tool built entirely in Blueprint to automate weapon data asset creation, validation, and correction. Built in Unreal Engine 5.7.

## Preview

![Weapon Asset Validator](Docs/tool_preview.png)

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

## Setup

1. Open the project in Unreal Engine 5.7
2. Open the Editor Utility Widget `EUW_WeaponAssetValidator`
3. Use the Create, Validate, and Fix buttons to manage weapon data assets

## Tech
- Unreal Engine 5.7
- 100% Blueprint — Editor Utility Widget, Data Assets, Enums
- No C++ or Python
