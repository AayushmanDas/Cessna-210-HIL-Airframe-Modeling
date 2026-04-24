# Cessna 210 Airframe Reconstruction & VLM Meshing
**NASA Variant Parametric Modeling**

<p align="center">
  <img src="media/mesh_render.png" width="700">
  <br>
  <i>Figure 1: Finalized Vortex Lattice Method (VLM) Mesh with 5,731 nodes.</i>
</p>

## Project Overview
This repository contains the 3D parametric reconstruction of a Cessna 210 Centurion airframe, modeled using NASA’s OpenVSP. The project bridges the gap between theoretical aircraft geometry and computational modeling for future telemetry integration.

## Technical Highlights
* **Geometric Fidelity:** Identified and corrected a critical instructional typo that listed the vertical stabilizer height at 2.94 ft; verified and adjusted to ~7.10 ft based on NASA 3-view ratios.
* **Numerical Discretization:** Generated a high-density mesh to verify geometric watertightness and surface continuity.
* **Computational Analysis:** Diagnosed numerical divergence (Kutta condition failure, $N_k=0$) caused by excessive Num-U discretization—optimized mesh parameters for future solver stability.

## Repository Structure
- **/model**: Contains the master `.vsp3` file and exported `.stp` CAD assembly.
- **/docs**: Contains the LaTeX source and the [Final Technical Project Log (PDF)](docs/Cessna_210_Project_Log.pdf).
- **/media**: High-resolution mesh renders and geometric previews.

## How to View
1. Install [OpenVSP](https://openvsp.org/download.php).
2. Open `model/Cessna210.vsp3`.
3. To view the mesh, navigate to `Analysis -> VSPAERO -> Prepare`.

---
*Developed by Aayushman Das, ETCE Dept., Jadavpur University (2026).*
