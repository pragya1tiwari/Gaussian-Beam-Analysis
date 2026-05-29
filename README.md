# Gaussian Beam Characterization and Parameter Estimation

## Overview

This project simulates a Gaussian laser beam intensity profile and demonstrates how experimental parameters can be extracted from noisy measurement data using nonlinear curve fitting techniques. The workflow mirrors real optical beam characterization methods used in photonics and experimental physics.

---

## Objective

To model a Gaussian beam, introduce realistic measurement noise, and recover key physical parameters (beam waist and peak intensity) using numerical optimization. The project also evaluates model quality using residual analysis and uncertainty estimation.

---

## Physical Model

The transverse intensity distribution of a Gaussian beam is given by:

I(x) = I₀ exp(-2x² / w²)

where:
- I₀: peak intensity
- w: beam waist (1/e² radius)
- x: transverse spatial coordinate

This model is widely used in laser optics and beam propagation analysis.

---

## Methodology

The analysis follows an experimental-style workflow:

1. Generate ideal Gaussian beam profile
2. Add synthetic Gaussian noise to simulate measurement conditions
3. Apply nonlinear curve fitting (SciPy optimization)
4. Extract beam parameters from noisy data
5. Evaluate fit quality using residual analysis
6. Estimate parameter uncertainty from covariance matrix

---

## Key Features

- Numerical simulation of optical beam profiles
- Curve fitting using nonlinear least squares
- Residual analysis for model validation
- Parameter uncertainty estimation
- Visualization of true vs measured vs fitted signals

---

## Tools & Libraries

- Python
- NumPy
- Matplotlib
- SciPy (curve fitting)

---

## Results & Interpretation

- The Gaussian model accurately reconstructs beam parameters from noisy data
- Residuals are randomly distributed, indicating a good model fit
- Parameter uncertainty quantifies confidence in extracted physical values
- The approach reflects standard experimental photonics data analysis workflows

---

## Scientific Relevance

This type of analysis is commonly used in:
- Laser beam profiling
- Optical metrology
- Photonics experiments
- Experimental physics data analysis

It demonstrates how theoretical models are validated against noisy experimental measurements.

---

## Limitations

- Assumes ideal Gaussian beam shape
- Assumes additive Gaussian noise only
- Does not account for optical aberrations or multimode effects
- Synthetic data used instead of real experimental measurements

---
