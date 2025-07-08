# HW-Module-Template

## Description

This repository is a template for hardware modules using KiCad, designed for clean, maintainable development with CI/CD pipelines generating and publishing production data automatically.

## Features
* Structured KiCad project (schematic, PCB)
* Clean repository: no production data stored
* GitHub Actions CI/CD pipeline:
  * Generates Gerber, BOM, and assembly files
  * Uploads artifacts to GitHub Releases
* Open Hardware license ready (CERN-OHL-S)

## Repository Structure

HW-Module-Template/
├── Hardware/              # KiCad project files
├── Doc/                   # Documentation exports
├── .github/workflows/     # CI/CD pipeline scripts
├── LICENSE
└── README.md

## Usage
1. Click “Use this template” on GitHub.
2. Clone your repository locally and open in KiCad.
3. Work on your schematic and PCB as usual.
4. Push your changes.
5. CI/CD will automatically generate production files and attach them to the latest GitHub Release.

## License

This project is licensed under CERN-OHL-S.

## Badges

![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/OE5XRX/<your-repo>/kicad-ci.yml?branch=main)
![GitHub Release](https://img.shields.io/github/v/release/OE5XRX/<your-repo>)
![License: CERN-OHL-S](https://img.shields.io/badge/license-CERN--OHL--S-blue)
![KiCad Supported](https://img.shields.io/badge/KiCad-supported-blue)
![Project Type](https://img.shields.io/badge/type-hardware-red)

## Contact

OE5XRX Amateur Radio Club
🌐 https://oe5xrx.org
✉️ info@oe5xrx.org
