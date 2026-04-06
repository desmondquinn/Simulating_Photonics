# Mie Scattering Simulations

This repository contains Python notebooks for simulating **Mie scattering** of spherical particles, including **dielectric and metal nanoparticles**. The simulations include **scattering efficiency calculations, multipole decomposition, and heatmap visualizations**.

<img src="https://github.com/user-attachments/assets/fe715407-30de-4ba1-8cb6-63e762d83224" width="45%" alt="mie_scattering_efficiency">

<img src="https://github.com/user-attachments/assets/a4618d4f-3e5a-4710-bbd5-50c14806d745" width="45%" alt="mie_scattering_efficiency_2">


## Repository Structure - Overview of notebooks

## 1) 'mie_heat_map.ipynb'

**Purpose:**  
Visualize the scattering efficiency of a dielectric particle as a function of particle radius and wavelength.

**Features:**  
- Computes Mie coefficients up to 2nd-order multipoles (dipole & quadrupole).  
- Generates heatmaps for total scattering and individual multipole contributions:  
  - Electric dipole (`a_1`)  
  - Electric quadrupole (`a_2`)  
  - Magnetic dipole (`b_1`)  
  - Magnetic quadrupole (`b_2`)  

**Parameters:**  
- Particle refractive index: `n = 3.5`  
- Medium refractive index: `n = 1`  
- Particle radius: `100–400 nm`  
- Wavelength: `300–1000 nm`  

## 2) 'mie_heat_map_2.ipynb'

**Purpose:**  
Visualize scattering efficiency of a dielectric particle as a function of wavelength and refractive index.

**Features:**  
- Computes Mie coefficients up to 2nd-order multipoles.  
- Generates heatmaps for total scattering and individual multipole contributions:  
  - Electric dipole (`a_1`)  
  - Electric quadrupole (`a_2`)  
  - Magnetic dipole (`b_1`)  
  - Magnetic quadrupole (`b_2`)  

**Parameters:**  
- Particle radius: `200 nm`  
- Refractive index: `1.3–4`  
- Wavelength: `300–1000 nm`  


## 3) 'mie_notebook.ipynb'

**Purpose:**  
Compute the scattering efficiency of dielectric and metallic (Ag) spherical particles as a function of wavelength.

**Features:**  
- Computes Mie coefficients for dielectric particles (radius 200 nm, `n = 3.5`).  
- Implements Drude-Lorentz model for silver nanoparticles.  
- Plots scattering efficiency vs wavelength for dielectric and metallic spheres.  

**Parameters:**  
- Dielectric particle: radius `200 nm`, refractive index `3.5`, medium `1`.  
- Metal particle (Ag): radius `20 nm`, Drude-Lorentz parameters from Rakic et al., 1998.  
- Wavelength:  
  - Dielectric: `300–1000 nm`  
  - Metal: `1–4.8 eV`  


## 4) 'multipole_decomposition.ipynb'

**Purpose:**  
Decompose the scattering efficiency of a particle into contributions from individual multipoles.

**Features:**  
- Computes total scattering and multipole contributions for electric and magnetic dipoles and quadrupoles.  
- Visualizes multipole contributions as line plots.  

**Parameters:**  
- Dielectric particle: radius `200 nm`, refractive index `3.5`, medium `1`.  
- Metal particle: radius `20 nm`, Drude-Lorentz parameters for Ag.  
- Wavelength range: dielectric `300–1000 nm`, metal `1–4.8 eV`.  


## Dependencies

The notebooks use the following Python libraries:

- `numpy` – for numerical computations  
- `scipy` – for special functions (`riccati_jn`, `riccati_yn`) used in Mie theory  
- `matplotlib` – for plotting and heatmaps  

Install dependencies via:

```bash
pip install numpy scipy matplotlib

