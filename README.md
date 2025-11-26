# Green Dense City - Visualization Tool

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

## Installation (Installer)

Pre-release installer (v0.2.0): https://github.com/dsjolie/GreenDenseCity/releases/download/v0.2.0/GronTatStad-Setup-0.2.0.exe

We ship a Windows installer in the dist repo that handles both the app and the volumetric data:

1. Run `GronTatStad-Setup-0.2.0.exe`.
2. Pick where to store data. The installer shows any existing path from `Documents\GronTatStad\DataPath.txt` and lets you keep it or reset to the default `%LOCALAPPDATA%\GronTatStad\VolumetricData`.
3. Choose dataset:
   - **Minimal (recommended first run)** – downloads `volumetric-data-v0.2.0-min.zip` into a subfolder `v0.2.0-min`.
   - **Full** – downloads all parts into `v0.2.0-full`.
4. Installer writes two pointers so the app can find the data:
   - `Documents\GronTatStad\DataPath.txt` → base data folder
   - `<InstallDir>\DTCC\dtcc_config.json` → mirrors the same base path

### Data layout

The base path (e.g. `%LOCALAPPDATA%\GronTatStad\VolumetricData`) contains versioned dataset folders:

```
VolumetricData\
  v0.2.0-min\   # minimal dataset
  v0.2.0-full\  # full dataset (all parts extracted here)
```

The app scans the base path for subfolders, so multiple dataset versions can coexist.

### Re-running the installer

You can rerun the installer to:
- Switch between minimal/full
- Change the data location
- Repair downloads

## Educational Materials

This tool is complemented by:
- Educational lectures
- Informational texts and guides
- Video content
- Research findings from the CityAirSim project

## Contributing to UN Sustainable Development Goals

This project contributes to three UN Global Goals:
- **Goal 3:** Good Health and Well-Being
- **Goal 11:** Sustainable Cities and Communities
- **Goal 15:** Life on Land

## Project Information

- **Duration:** 2024–2026
- **Budget:** 2 MSEK
- **Funding:** Formas

## Learn More

For detailed information about the research project, visit:
https://www.ivl.se/english/ivl/our-offer/research-projects/air/green-dense-city.html

## License

*License information to be added.*

## Contact

*Contact information to be added.*

---

© 2024-2026 IVL Swedish Environmental Research Institute and partners
