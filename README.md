

# Cognitive Ability Screener (CAI)

## Overview
This repository contains a lightweight, fully client-side cognitive ability screener. The project originated when my 7-year-old asked about her IQ, and I discovered a lack of scientifically grounded, free, and privacy-respecting cognitive assessments online. 

Rather than a standard commercial "IQ test," this tool generates an algorithmically adaptive **Cognitive Ability Index (CAI)** based on the Cattell-Horn-Carroll (CHC) theory of cognitive abilities.

## Key Features
* **Zero Data Transmission:** 100% client-side logic (HTML/JS/Tailwind). No tracking, no external server calls. Inherently COPPA and GDPR-K compliant.
* **Algorithmically Adaptive:** Utilizes difficulty-weighted scoring (IRT-lite) to adjust question complexity dynamically based on user performance.
* **Age-Normed:** Applies domain-specific age growth/decay formulas to map raw ability estimates against chronological age.
* **Reliability Tracking:** Calculates internal consistency metrics (maximum streak vs. total correct) to flag random guessing.

## Assessment Domains

| Phase | Cognitive Domain | CHC Construct | Task Mechanics |
| :--- | :--- | :--- | :--- |
| **Phase 1** | Quantitative Reasoning | Gq | Algorithmic number sequence extrapolation |
| **Phase 2** | Fluid Spatial Logic | Gf | 3x3 matrix pattern abstraction (Raven's style) |
| **Phases 3 & 4**| Working Memory | Gwm | Forward and backward visuospatial span (Corsi block-tapping) |
| **Phase 5** | Processing Speed | Gs | Timed symbol target identification (WAIS Symbol Search style) |

## Usage
Simply clone the repository and open `index.html` in any modern web browser. No build steps, dependencies, or server environments are required.

```bash
git clone [https://github.com/yourusername/your-repo-name.git](https://github.com/yourusername/your-repo-name.git)
cd your-repo-name
open index.html
