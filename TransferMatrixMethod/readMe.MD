# Thin Film Optics Simulation using Transfer Matrix Method (TMM)

## 📌 Overview

This project simulates the optical properties (Reflection, Transmission, and Absorption) of thin metal films using the Transfer Matrix Method (TMM). The focus is on comparing **gold (Au)** and **chromium (Cr)** thin films for applications in optical imaging and microfluidic devices.


The simulations explore:

- Angular dependence (0–90° incidence)
- Wavelength dependence (visible spectrum: 400–800 nm)
- Thickness dependence (30 nm vs 50 nm)
- Multi-layer systems (Au with Cr adhesion layer)



## ⚙️ Methodology

The simulations are performed using the Python package:
- `tmm` → coherent transfer matrix calculations via `coh_tmm`



## 🧪 Materials & Optical Constants

Optical constants (n, k) are taken from:

- Johnson & Christy dataset  
- Source: refractiveindex.info  

### Materials:
- Gold (Au)
- Chromium (Cr)

Datasets:
- `gold-Johnson.csv`
- `chrome-Johnson.csv`



## 📊 Simulations Performed

### 1. Angular Dependence (808 nm, 532 nm)

- Incident angle: 0° to 90°
- p-polarized light
- Comparison between Au and Cr films

### 2. Spectral Response (Visible Range)

- Wavelength range: 400–800 nm
- Normal incidence (0°)
- Film thickness:
  - 50 nm Au
  - 30 nm Au
  - 30 nm Cr

### 3. Multilayer System

- Cr (adhesion) layer + Au layer  
- Evaluates realistic fabrication conditions  



## 📈 Key Results

- **Chromium (Cr) films exhibit lower transmission** in the visible spectrum compared to gold (Au).  
- For transmission-based imaging, reducing the thickness of Au alone is insufficient; **reducing the Cr layer thickness is essential to improve imaging performance**.  



## 📦 Requirements

```bash
pip install numpy matplotlib pandas tmm
