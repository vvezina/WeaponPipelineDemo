# Weapon Asset Validator

## Why

I built this tool to improve my Unreal tools/pipeline skills for my portfolio.  
I wanted something simple but practical, so I focused on validating DataAssets since they’re commonly used and easy to mess up in production.

## What it does

This tool scans the project for all available DataAssets.

From there, it can:

- Validate naming conventions  
- Detect invalid data (None / zero values)  
- Automatically fix issues directly inside the editor based on default values  
- Creating new DataAssets based on a predefined structure  

Example: creating a new weapon like a Rocket Launcher will automatically follow the correct structure and default values.

## <u>**Notes**</u>

- Built to work on an existing dataset inside the project  
- Designed to avoid manual checking and reduce errors when creating new assets  
- Designed to run entirely in Blueprint for fast iteration inside the editor  

## Preview

![Weapon Asset Validator](Docs/tool_preview.png)

## Setup

1. Open the project in Unreal Engine 5.7  
2. Open the Editor Utility Widget `EUW_WeaponAssetValidator`  
3. Use the Create, Validate, and Fix buttons to manage weapon data assets  

## Tech

- Unreal Engine 5.7  
- 100% Blueprint — Editor Utility Widget
- No C++ or Python  
