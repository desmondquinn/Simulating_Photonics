---

# Fourier Optics: Angular Spectrum Method

## `Diffraction-Pinhole-Aperture.ipynb`

**Purpose:**  
Simulate diffraction patterns of light from a pinhole aperture using the Angular Spectrum method, and demonstrate backward propagation to reconstruct the aperture image.

**Features:**  
- Computes the diffraction pattern at a given distance from a pinhole.  
- Uses the Fourier Transform (FFT) to implement the Angular Spectrum method.  
- Demonstrates forward and backward propagation of light waves.  
- Reconstructs the original aperture from the propagated field.  

**Parameters:**  
- Spatial grid: `-2 mm ≤ X,Y ≤ 2 mm`, `2000 × 2000` points  
- Pinhole radius: `r = 0.55 mm`  
- Wavelength of light: `λ = 532 nm`  
- Propagation distance: `z = ±20 cm`  
- Computation: Angular Spectrum via `FFT` and `IFFT`  
