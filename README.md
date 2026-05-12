# HW-Module-Template

GitHub "Use this template" scaffold for new hardware module repositories under OE5XRX. New modules cloned from this template start pre-wired to the shared CI infrastructure at [`OE5XRX/HW-Module-CI`](https://github.com/OE5XRX/HW-Module-CI).

## Quickstart for new modules

1. Click **"Use this template"** on GitHub to create a new module repo (e.g., `HW-Module-Acme`).
2. Clone the new repo locally.
3. Replace `LICENSE` if your license differs from CERN-OHL-S 2.0.
4. Create your KiCad project at the repo root. The `.kicad_pro`, `.kicad_sch`, and `.kicad_pcb` can be named anything — the shared CI auto-detects the basename. Convention: name them after the module (e.g., `Acme.kicad_pro`).
5. Fill in `doc/index.md`:
   - Replace `<NAME>` with the module's display name (e.g., `Acme`).
   - Update `nav_order` to position it correctly on the hardware overview page.
   - Replace `Some Text` with the module description, voltage tables, etc.
   - Output paths already use `{{ site.data.project.name }}` — leave those as-is; CI fills in the auto-detected KiCad basename at build time.
6. Commit and push. On the first push to `main`, CI auto-runs:
   - `KiBot Check` — ERC + DRC preflight
   - `Create Debug Docs` — publishes preview to the repo's `gh-pages` branch
7. On the first GitHub release: `Create Release Docs` deploys versioned docs to `OE5XRX.github.io` and pushes BOM to InvenTree.

## What this template provides

- `.github/workflows/` — 3 thin wrappers that `uses: HW-Module-CI@main`
- `doc/index.md` — Jekyll page scaffold (replace `<NAME>` + content)
- `3d-models/`, `symbols/`, `footprints/` — empty subdirs for optional KiCad libraries
- `LICENSE` — CERN-OHL-S 2.0
- `README.md` — this file (overwrite for your module)

## What's intentionally NOT in this template

KiBot configs, Python scripts (BOM export, InvenTree sync, stencil PNG), Jekyll config, Gemfile, doc assets (favicon, logo) — all of these live in [`OE5XRX/HW-Module-CI`](https://github.com/OE5XRX/HW-Module-CI) and are pulled in at CI-runtime. Do not copy them here.

## License

[CERN-OHL-S-2.0](https://choosealicense.com/licenses/cern-ohl-s-2.0/) by default; replace `LICENSE` if your module needs a different license.

## Contact

OE5XRX Amateur Radio Club  
🌐 https://oe5xrx.org  
✉️ info@oe5xrx.org
