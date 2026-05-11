# Green Dense City — Visualization Tool

> ℹ️ **The application UI is in Swedish.** This README is in English; the installer and the app itself ("GrönTätStad") run in Swedish.

An interactive visualization tool for exploring how urban design, buildings, and green spaces contribute to healthy and sustainable city environments.

## About the Project

Green Dense City is a research initiative funded by Formas, aimed at increasing public understanding of how buildings and green spaces can be used to create healthy, green living environments in densified urban areas.

The project addresses critical questions about urban development:
- How can we design dense cities that remain healthy and sustainable?
- What role do green spaces play in urban quality of life?
- How do building design choices affect air quality and climate?

This visualization tool combines research data from the CityAirSim project with educational materials to help users explore the relationships between urban design choices and environmental outcomes.

## Project Partners

- **IVL Swedish Environmental Research Institute** (Lead)
- **University West**
- **University of Gothenburg**
- **Gothenburg Botanical Garden**

## Features

The visualization tool allows users to:
- Explore different urban design scenarios
- Understand relationships between building density and environmental quality
- Visualize the impact of green space integration
- Learn about air quality and climate effects of urban design decisions

## Installation

End users don't run the packaged app directly. A small **launcher** handles downloading and updating the app and its volumetric datasets, and then starts the visualization.

### Recommended (Windows)

Install **v0.2.6** using the Windows installer, and let the launcher self-update to the latest version after the first start:

1. Download **[GronTatStad-Setup-0.2.6.exe](https://github.com/dsjolie/GreenDenseCity/releases/download/v0.2.6/GronTatStad-Setup-0.2.6.exe)** from the [v0.2.6 release](https://github.com/dsjolie/GreenDenseCity/releases/tag/v0.2.6).
2. Run the installer. It installs the launcher and writes the data-path pointer the app needs.
3. Launch **GrönTätStad** from the Start menu. The launcher will:
   - Check for a newer launcher build and update itself if available.
   - Offer to download the latest app build and volumetric dataset.
   - Start the visualization once everything is in place.

> Why 0.2.6 rather than the absolute latest? It is the most recent release that ships a Windows installer. Newer app builds are picked up automatically by the launcher after install.

### macOS

A macOS (Apple Silicon) build of the launcher is published alongside the app releases. There is no installer yet — download the latest `GronTatStad-Launcher-*-mac-arm64.zip` from the [Releases page](https://github.com/dsjolie/GreenDenseCity/releases), unzip it, and move the `.app` into `/Applications` before launching. The launcher then handles app and data downloads as on Windows.

### What the launcher manages

- **Launcher binary** — self-updates from this repository's Releases.
- **App binary** — downloaded into a per-user location and updated when a new release is published.
- **Volumetric datasets** — versioned dataset folders (e.g. `v0.2.2-lowres`, `v0.2.0-full`) installed under a single base directory. Multiple dataset versions can coexist; the app scans the base directory and lists every dataset it finds.

## Learn More

For detailed information about the research project, visit:
https://www.ivl.se/english/ivl/our-offer/research-projects/air/green-dense-city.html

---

© 2024-2026 IVL Swedish Environmental Research Institute and partners
