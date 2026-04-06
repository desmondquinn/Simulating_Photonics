# 1D FDTD Simulation

This repository contains a **1D Finite-Difference Time-Domain (FDTD) simulation** of electromagnetic wave propagation in free space with a single dielectric slab. The simulation is implemented from scratch to showcase the physics of wave propagation and demonstrate a custom numerical solver.

https://user-images.githubusercontent.com/21221799/152292548-91fd325a-07b3-4791-a4f1-4b9dbb1e7765.mp4


## 🔹 Features
- Gaussian pulse source for excitation  
- Perfectly absorbing boundary conditions (PML-like)  
- Single dielectric slab embedded in free space  
- Animated visualization of the `Ey` field evolution  


## 🔹 Simulation Description
A Gaussian pulse is injected at the left end of the grid. It travels through free space and interacts with a material of higher refractive index. The edges of the dielectric slab (material 2) are marked by two straight lines in the animation. The reflection at each of the interfaces is seem in the visualisation along with the phase shift.


## 🔹 Usage

Run the Python script:

```bash
python fdtd_1d.py

## for dependencies
pip install numpy matplotlib ffmpeg
