# PCC--ARBM Tendon Allocation for Motor-Driven Continuum Arms

This repository contains supplementary material, simulation figures, and videos associated with the paper:

**"A Control Allocation Strategy for Tendon-driven Arms Modeled Via the Augmented Rigid Body Approach"**

The paper presents a control-allocation framework for motor-driven tendon-actuated continuum arms modeled using Piecewise Constant Curvature (PCC) and Augmented Rigid Body Model (ARBM) formulations. The proposed framework connects curvature-space control efforts with physically realizable tendon tensions and motor torques.

## Overview

The proposed framework combines:

- reduced-order PCC/ARBM modeling,
- curvature-space control,
- tendon-force allocation,
- non-negative tendon tension constraints,
- motor--tendon dynamics including spool kinematics, elasticity, damping, and motor dynamics.

This repository provides supplementary simulation material for both the planar 2D and spatial 3D cases.

## Repository structure

```text
supplementary/              Supplementary PDF material.
simulations/planar_2d/      Figures and videos for the planar three-segment case.
simulations/spatial_3d/     Figures and videos for the spatial 3D case.
parameters/                 Simulation parameter summary.

```markdown
## Simulation cases

- [Planar 2D case](./simulations/planar_2d/): three-segment tendon-driven continuum arm controlled through scalar curvature coordinates.
- [Spatial 3D case](./simulations/spatial_3d/): single 3D PCC segment controlled through bending-plane orientation and bending magnitude.

Each simulation folder contains a dedicated README file with a short description of the setup, the reference trajectories, the corresponding figures, and the available animations.

## Simulation parameters

The main geometric and motor--tendon parameters used in the simulations are summarized in:

- [Simulation parameters](./parameters/simulation_parameters.md)

## Code availability

The implementation code is not included in this public repository. This repository is intended to provide supplementary documentation, simulation figures, videos, and parameter information associated with the paper.

## Citation

If you use this material, please cite the corresponding paper:

```bibtex
@inproceedings{pineda2026allocation,
  title     = {A Control Allocation Strategy for Tendon-driven Arms Modeled Via the Augmented Rigid Body Approach},
  author    = {Pineda, Rogelio and Espinosa, Isaac and Flores, Gerardo and Becerra, Hector M.},
  booktitle = {Proceedings of the 23rd IFAC World Congress},
  year      = {2026}
}