# PICNO_S: Physics-Informed Framework for Solving Parameterized Partial Differential Equations with Continuous Dependence

## Overview

Solving parameterized PDEs is fundamental in fields such as climate modeling, where repeated solutions under varying parameters and initial/boundary values are required. Traditional numerical solvers, while accurate, are computationally prohibitive for real-time or large-scale applications. Deep-learning-based solvers such as PINNs, DeepONet, and FNO improve efficiency but suffer from costly retraining and high data demands. Building on the continuous dependence of PDE solutions on parameters and initial/boundary values, we develop the Continuous Neural Operator (CNO), which captures this dependence through a latent representation. Based on this foundation, we develop PICNO and PICNO-S, which use explicit encoding and differentiability dependence to enhance accuracy and stability. Experiments show that CNO achieves test MSEs 1-2 orders of magnitude lower than DeepONet and FNO with limited labeled data, while PICNO-S outperforms PI-DeepONet by about 2 orders of magnitude. On the Burgers equation, when the number of configurations exceeds 30, PICNO-S training cost matches the cumulative runtime of FDM, while delivering numerical-level accuracy with negligible inference time for new configurations. These results highlight the potential of our models for real-world PDE applications.

## Applications

We showcase the effectiveness of PICNO_S through several examples, including:
- The diffusion equation
- The Wave equation
- The burgers equation

These case studies highlight the robustness of PICNO_S in a variety of scenarios.
