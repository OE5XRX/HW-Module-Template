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

```
HW-Module-Template/
├── .github/workflows/     # CI/CD pipeline scripts
├── doc/                   # Documentation exports
├── hardware/              # KiCad project files
│   ├── symbols/           # Local symbol library (if needed)
│   ├── footprints/        # Local footprint library (if needed)
│   ├── 3d-models/         # STEP/WRL files (optional)
├── LICENSE
└── README.md
```

## Usage
1. Click “Use this template” on GitHub.
2. Clone your repository locally and open in KiCad.
3. Work on your schematic and PCB as usual.
4. Push your changes.
5. CI/CD will automatically generate production files and attach them to the latest GitHub Release.

## License

This project is licensed under [CERN-OHL-S-2.0](https://choosealicense.com/licenses/cern-ohl-s-2.0/).

## Badges

![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/OE5XRX/<your-repo>/kicad-ci.yml?branch=main)<br>
![GitHub Release](https://img.shields.io/github/v/release/OE5XRX/<your-repo>)<br>
![License: CERN-OHL-S](https://img.shields.io/badge/license-CERN--OHL--S--2.0-blue)<br>
![KiCad Supported](https://img.shields.io/badge/KiCad-supported-blue)<br>
![Project Type](https://img.shields.io/badge/type-hardware-red)<br>

## Contact

OE5XRX Amateur Radio Club<br>
🌐 https://oe5xrx.org<br>
✉️ info@oe5xrx.org<br>
