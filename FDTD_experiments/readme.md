# Photonic Circuits

This sub-repository explores how light can be controlled in photonic circuits using micro- and nanostructures. 

## 2D Waveguide Created by a Line Defect in a Photonic Crystal 
### Notebook: '2d-PhC_waveguide-v2.ipynb'

<img src="phc_waveguide.gif" alt="2D Photonic Crystal Waveguide Animation" width="60%">

This notebook demonstrates how a **2D photonic crystal** made of GaAs cylinders can guide light along a **line defect**:

- **Photonic Crystal Setup** : A periodic lattice of high-refractive-index cylinders forms the photonic crystal. By removing a row of cylinders at the center, a waveguide channel is created along the x-axis.

- **Gaussian Source** : A Gaussian pulse is launched into the waveguide to excite electromagnetic modes.

- **Simulation** : The simulation uses **Meep (FDTD)** to compute how the electric field evolves over time. Absorbing boundary conditions (PML layers) prevent artificial reflections.

- **Visualization** : Field snapshots are collected and animated to show how light propagates along the waveguide. The animation highlights the confinement and guidance of the field within the defect channel.

## Applications
- Guiding light in photonic circuits    
- Exploring photonic crystal-based devices such as filters, bends, and cavities   
