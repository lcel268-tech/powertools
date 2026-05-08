# PowerTools — ECU Tuning Toolbox

[![Website](https://img.shields.io/badge/Website-ptools.site-blue)](http://ptools.site)
![Language](https://img.shields.io/badge/Language-Python%2FTypeScript-green)

> A power data analysis platform built for automotive tuners. Generate dyno graphs online, analyze CSV data streams, and match ECU files.

## Features

### 🔧 Dyno Graph Generation (YourDyno)
- Upload YourDyno dyno CSV files to auto-generate professional horsepower / torque curves
- Auto-detect peak power (HP) and peak torque (TQ)
- Multi-file overlay comparison with custom brand logo support
- Wheel horsepower vs engine power delta analysis
- Works entirely online — no installation required

### 📊 CSV Data Stream Analysis
- Visualize data logs from MHD / Bootmod3 / Autotuner / Ktuner / VCDS
- Signal filtering, denoising, and outlier removal
- Built for modified vehicle power testing and diagnostics

### 🔍 ECU File Matching
- Fast BMW ECU A2L / XDF file matching
- Bosch MED17 / EDC17 / MG1 / MD1 checksum repair
- XDF → WinOLS JSON format conversion
- WinOLS NOREAD digital signature removal

### 🛠 Tuning Data Lookup
- 5,000+ vehicle tuning profiles
- Covers BMW, Audi, VW, Porsche, Mercedes, and other major brands
- Stock horsepower / torque vs tuned output comparison

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

---

*PowerTools — Make your dyno data speak.*