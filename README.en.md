# PowerTools — ECU Tuning Toolbox

[![Website](https://img.shields.io/badge/Website-ptools.site-blue)](http://ptools.site)
![Language](https://img.shields.io/badge/Language-Python%2FTypeScript-green)

> A power data analysis platform built for automotive tuners. Generate dyno graphs online, analyze CSV data streams, match ECU files, and tune Honda ECUs in the browser.

## Features

### 🔧 Dyno Graph Generation (YourDyno)
- Upload YourDyno dyno CSV files to auto-generate professional horsepower / torque curves
- Auto-detect peak power (HP) and peak torque (TQ)
- Multi-file overlay comparison with custom brand logo support — logos persist permanently after one upload
- Professional report format: auto-inferred cylinder count, ModSpec modification list, fuel type dropdown (Gasoline / Diesel / E85 / E50 / E30 / Methanol / Race Gas / Other)
- Three smoothing modes: Off / Standard (< 0.01% peak deviation) / Strong (~0.05%)
- Wheel horsepower vs engine power delta analysis
- Works entirely online — no installation required

### 📈 Interactive Dyno Curve Analysis
- Live cursor tracking: hover to see horsepower / torque at any RPM in real time
- Overlay multiple curves with independent cursor tracking per curve
- Drag-and-drop CSV upload, no login required
- Dark / Light / Warm themes, logo overlay, PNG export
- Mobile-responsive layout

### 📊 CSV Data Stream Analysis
- Visualize data logs from MHD / Bootmod3 / Autotuner / Ktuner / VCDS
- **Direct Autotuner datalog link reading** — paste the web datalog URL, no CSV download needed
- 8mb-flash Datalog CSV format support (with timestamp parsing fixes)
- WOT (wide-open throttle) segment auto-detection with highlighted acceleration zones
- Engine performance panel: max power (kW@RPM), max torque (Nm@RPM), peak boost (bar), knock count, acceleration segment count
- Signal filtering, denoising, and outlier removal
- Built for modified vehicle power testing and diagnostics

### 🔍 ECU File Matching
- Fast BMW ECU A2L / XDF file matching — B48 / B58 / S55 / S58 / S63
- **MHD XDF matcher**: 105 ECU IDs auto-matched (.bin / .rom upload, 12-digit exact + 8-digit fuzzy matching)
- Bosch MED17 / EDC17 / MG1 / MD1 checksum repair
- **XDF → WinOLS JSON converter**: parses all map definitions, optional BIN upload to read actual values, built-in conversion validation
- WinOLS NOREAD digital signature one-click removal

### 🏎 Honda-HEX Online Honda ECU Tuning
- Upload a stock bin file, modify and download directly in the browser — fully client-side
- Auto ECU version detection: Civic 8th gen R18A (10 versions), Fit GE8 L15A, Fit GK5 L15B
- Tuning options: ignition timing / MAF correction / rev limiter / throttle response / idle speed / knock sensitivity
- L15B advanced recipes: tachometer scaling, VTEC engagement point, fuel cut, speed limiter removal, VTC angle optimization, cruise control activation

### 🛠 Tuning Data Lookup
- Stock power data for 59 brands and 8,000+ engine configurations
- Covers BMW, Audi, VW, Porsche, Mercedes, Ford, Volvo plus Japanese, Korean, and Chinese brands
- Stock horsepower / torque vs Stage 1 / Stage 2 tuned output comparison
- Some models include ECU part numbers, flashing tool recommendations, and dyno-verified curves

## Quick Start

Visit [ptools.site](http://ptools.site) to get started — no registration needed.
Demo account available, 5 minutes to your first graph.

## Tech Stack

| Component | Technology |
|-----------|------------|
| Frontend  | Next.js / TypeScript / Canvas |
| Backend   | Python Flask |
| Toolchain | rx14-cli (C++), OpenCLI |
| Data      | Feishu Multidimensional Tables, JSON |

## Links

- Website: [ptools.site](http://ptools.site)
- Changelog: [/updates](https://ptools.site/updates)

## Who It's For

- **Shop techs** — generate customer dyno reports in seconds
- **ECU tuners** — data analysis and file matching on the fly
- **Fleet managers** — compare and archive power data across multiple vehicles
- **Honda owners** — tune stock bins online, no professional hardware required

---

*PowerTools — Make your dyno data speak.*
