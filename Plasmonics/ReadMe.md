
# Plasmonics – FDTD Simulation (Meep)

This module contains a simple Finite-Difference Time-Domain (FDTD) simulation of electromagnetic field interactions in a nanoscale system using the Meep library.

The setup is designed as a minimal example for studying plasmonic behavior in a metallic nanoparticle, with a focus on field response at optical frequencies.


## 📌 Overview

The simulation solves Maxwell’s equations in the time domain using Meep. A broadband Gaussian source excites the system, and the resulting electric field is recorded in the frequency domain.

This simulation setup was used to observe Localized surface plasmon resonances (LSPR) and Near-field enhancements of a silver nanoparticle.

<img src="https://github.com/user-attachments/assets/8f908887-b97f-413c-9f57-f8bcf5f41d76" width="40%">



## ⚙️ Simulation Details

- **Method:** Finite-Difference Time-Domain (FDTD)  
- **Library:** Meep  
- **Resolution:** 300 pixels / unit length  
- **Cell size:** 0.8 × 0.8 × 0.8  
- **Boundary conditions:** Perfectly Matched Layers (PML)  
- **Symmetry:** Mirror symmetry along Y-axis  

### Source
- Gaussian source centered at:
  - Wavelength ≈ 0.354 μm  
- Polarization: Ex  
- Planar source spanning XY plane  

### Frequency-domain analysis
- Discrete Fourier Transform (DFT) used to extract steady-state field  
- Field recorded at simulation center  


## 🚀 How to Run

### 1. Install dependencies
```bash
pip install meep numpy matplotlib
