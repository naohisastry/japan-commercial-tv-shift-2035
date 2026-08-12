# Commercial TV Shift 2035 (TV-Shift 2035)
### Japan Top 5 Commercial TV Broadcasters: Revenue Structure Transformation Simulation (2015–2035)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-Single%20Page%20App-orange.svg)](#)
[![Chart.js](https://img.shields.io/badge/Charts-Chart.js-FF6384.svg)](#)

An interactive, zero-dependency financial simulation dashboard analyzing the long-term revenue transition of Japan's Top 5 commercial television networks from traditional linear broadcasting to digital streaming, IP monetization, and non-broadcasting operations.

---

## 🔮 Overview

As terrestrial linear TV advertising undergoes a structural secular decline across Japan, commercial broadcasters are actively diversifying their core revenue streams. 

This simulation model bridges statutory securities disclosures (Yuka Shoken Hokokusho actuals: FY2015–FY2026) with long-term econometric forecasting models (FY2027–FY2035) using a **"Differential Modeling Approach"**. It dynamically isolates digital streaming and IP licensing from legacy broadcasting operations, providing executive-level strategic visibility into the structural transformation of Japan's commercial media landscape.

### Covered Broadcasters
1. **Nippon Television Holdings (NTV / 9404.T)**
2. **TV Asahi Holdings (EX / 9409.T)**
3. **TBS Holdings (TBS / 9401.T)**
4. **TV Tokyo Holdings (TX / 9413.T)**
5. **Fuji Media Holdings (CX / 4676.T)**
* **Top 5 Broadcasters Aggregate (Total)**

---

## 🚀 Key Features

* **📦 100% Zero-Dependency Standalone Package**:
  Fully portable, single-file HTML applications. Runs instantly in any standard browser without local web servers (`localhost`), database setups, or node modules.
* **🔮 Mathematical Dynamic Venn Diagram**:
  Circle radii, horizontal overlap, and vertical separation are driven 100% dynamically by financial metrics:
  * **Broadcasting ⇔ Digital/Related (Horizontal Overlap)**: Expands dynamically with each broadcaster's *Digital Streaming Ratio* (TVer, SVOD).
  * **Broadcast-Related ⇔ Non-Broadcasting (Vertical Distance)**: Separates based on the proportion of pure non-media assets (e.g., Sankei Building real estate, Granvista hotels, PLAZA lifestyle retail).
* **📊 Dual Interactive Analytics**:
  * Stacked Area Revenue Composition Chart (JPY Millions)
  * Segment Percentage Transition Shift Chart (%)
  * Full Historical & Forecast Numerical Data Grid
* **📷 Slide-Export Engine**:
  Exports publication-ready, white-background SVG/PNG charts formatted specifically for PowerPoint / Keynote presentation decks.
* **🌐 Dual-Language Support**:
  Full native Japanese and English versions.

---

## 📁 Repository Structure

```text
├── TV-Shift2035_Revenue_Transition_Simulator_EN.html  # Standalone English Simulator (Single-file)
├── TV-Shift2035_Revenue_Transition_Simulator.html     # Standalone Japanese Simulator (Single-file)
├── index.html                                        # Source HTML (Japanese)
├── index_en.html                                     # Source HTML (English)
├── styles.css                                        # Core Glassmorphic Design System
├── app.js                                            # Japanese UI Logic & Strategic Insights
├── app_en.js                                         # English UI Logic & Strategic Insights
├── data.js                                           # Time-Series Database (2015-2035)
├── generate_aligned_forecast.py                      # Data Harmonization & Differential Modeling Engine
├── build_dist.py                                     # Multi-Language Standalone Packager
└── README.md                                         # Project Documentation
```

---

## 💻 How to Run Locally

Simply double-click either standalone HTML file to launch immediately in your preferred browser:
* **English Version**: Double-click `TV-Shift2035_Revenue_Transition_Simulator_EN.html`
* **Japanese Version**: Double-click `TV-Shift2035_Revenue_Transition_Simulator.html`

To rebuild standalone packages from source after editing styles or data:
```bash
python build_dist.py
```

---

## 🌐 Deploy to GitHub Pages (Live Web Access)

You can host this interactive simulation on the web via GitHub Pages in 3 simple steps:

1. **Push this repository to GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Commercial TV Shift 2035 Simulator"
   git branch -M main
   git remote add origin https://github.com/<YOUR-USERNAME>/<YOUR-REPO-NAME>.git
   git push -u origin main
   ```
2. **Configure GitHub Pages**:
   * Navigate to your GitHub repository -> **Settings** -> **Pages**.
   * Under **Build and deployment** -> **Source**, select `Deploy from a branch`.
   * Set the branch to `main` and folder to `/(root)`, then click **Save**.
3. **Access Live Links**:
   * **Japanese Dashboard**: `https://<YOUR-USERNAME>.github.io/<YOUR-REPO-NAME>/index.html`
   * **English Dashboard**: `https://<YOUR-USERNAME>.github.io/<YOUR-REPO-NAME>/index_en.html`
   * *(Or open standalone files directly from the repository)*

---

## 📈 Methodology & Data Lineage

1. **Linear TV Ad Baseline (Broadcasting)**:
   Fixed to terrestrial linear advertising revenue (Time + Spot), declining along empirical econometric forecast vectors through 2035.
2. **Broadcast-Related Differential Allocation**:
   Residual broadcast-related revenues are decomposed into *Digital/Streaming* (TVer, Hulu, FOD, YouTube, TELASA) and *Traditional Peripheral* (CS/BS broadcasting, contract production, traditional music rights).
3. **Two-Tier Growth Model**:
   * Digital/IP segments grow at broadcaster-specific annual CAGRs (+5.0% to +8.0%).
   * Traditional peripheral businesses are modeled conservatively at 0.0% YoY.
4. **Pure Non-Media Segment Isolation**:
   Real estate leasing (Akasaka Sacas, Roppongi Hills leases, Sankei Building), fitness gyms (Tipness), and hotel operations are isolated into Non-Broadcasting to ensure core media synergy is measured without distortion.

---

## ⚖️ License & Disclaimer

* Code is open-sourced under the [MIT License](LICENSE).
* Financial actuals are derived from publicly available annual securities reports (Yuka Shoken Hokokusho). Forecast figures are econometric scenario projections for strategic research and simulation purposes.
