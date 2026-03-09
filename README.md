# Corrosion-Aware Structural Health Monitoring

**Corrosion-Aware Structural Health Monitoring via Modal Analysis of a 3-Story Shear Frame**

This project presents a Python-based structural health monitoring workflow for a 3-story shear frame, with a focus on how **live load variation** and **corrosion-induced section loss** affect modal properties. The implementation uses classical structural dynamics and numerical linear algebra to evaluate changes in **mass**, **stiffness**, **natural frequencies**, and **mode shapes**.

The project was developed in Python using **NumPy**, **SciPy**, and **Matplotlib**, and is organized as a computational study suitable for structural analysis, condition assessment, and damage-sensitive modal investigation.

## Project Summary

This repository includes a modal-analysis-based structural health monitoring tool that:

- models a **3-story shear frame**
- studies the effect of **live load variation** on modal properties
- evaluates the impact of **corrosion** on section properties and structural response
- compares **healthy** and **corroded** structural states
- visualizes the resulting changes in frequencies and mode shapes

## Key Features

- **Modal analysis of a 3-story shear frame**
- **Live load sensitivity analysis**
- **Corrosion-aware section property update**
- **Centroid and moment of inertia recalculation**
- **Mass and stiffness matrix formulation**
- **Healthy vs corroded structural comparison**
- **Visualization of modal property changes**
- **Verification-oriented workflow** for selected calculations

## Methodology

The notebook is divided into three main parts:

### 1. Live Load Variation
The first part studies how changes in the live load portion affect the dynamic properties of the structure. The mass matrix is updated for different live load levels, and modal analysis is performed to compute:

- circular frequencies
- natural frequencies
- mode shapes

### 2. Corrosion Effects
The second part introduces corrosion into the structural model by reducing the flange thickness of a steel section. The workflow then recomputes:

- modified section geometry
- centroid location
- moment of inertia
- lost mass due to corrosion

These updated properties are then incorporated into the structural model.

### 3. Structural Health Monitoring Comparison
The final part compares two structural states:

- **Healthy structure**: no corrosion
- **Corroded structure**: reduced section stiffness and mass

The comparison highlights how damage affects:

- mass matrix
- stiffness matrix
- modal frequencies
- mode shapes

## Repository Structure

```text
Corrosion-Aware-Structural-Health-Monitoring/
├── README.md
├── main.ipynb
└── ReadMe_Structural Dynamics.pdf
