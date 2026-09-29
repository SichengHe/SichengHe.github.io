---
layout: archive
title: "Research"
permalink: /research/
author_profile: false
redirect_from:
  - /resume
---

<div class="lab-callout">
<strong>Our mission:</strong> To develop structured and differentiable representations of complex dynamical systems that enable scalable analysis, physical insight, and optimal design.
</div>

Our research is organized around three pillars: (1) **structured representations** of nonlinear dynamics, (2) **operator-theoretic analysis** and interpretable reduced coordinates, and (3) **optimization, control, and learning** of dynamical systems.

## Research highlight: transonic buffet

Transonic buffet—self-sustained shock and shear-layer oscillations—limits the cruise envelope of modern transport aircraft and emerges through a **Hopf bifurcation** of the steady flow.
Led by Ph.D. student Rohit Kanchi, we predict buffet onset from first principles with **linear stability analysis (LST)** of the steady base flow, and we developed a **coupled adjoint** that computes the sensitivity of the dominant LST eigenvalue with respect to a large number of shape design variables.
A buffet-constrained drag minimization of the OAT15A supercritical airfoil achieves a **22.4% drag reduction** while satisfying the LST-based buffet constraint.
This work received the **2026 AIAA MDO Best Student Paper Runner-Up** award.

We are extending the approach to three-dimensional buffet on swept wings.
The simulation below was computed using [ADflow](https://github.com/mdolab/adflow), a state-of-the-art RANS-based finite-volume solver, on NASA's [Common Research Model (CRM)](https://commonresearchmodel.larc.nasa.gov/) wing in the wing-only configuration, at **Mach 0.85**, **angle of attack 4.2 deg**, and **Reynolds number 5 million**.

<figure class="lab-figure">
  <video controls playsinline preload="metadata" poster="../images/research/transonic_buffet_3d_tile.png" style="width: 100%; max-width: 1100px; background: #000; border: 1px solid #d8d8d8; border-radius: 6px;">
    <source src="../assets/videos/transonic-buffet-3d-crm.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <figcaption>A tiled view of the 3D buffet dynamics on the CRM wing showing the Q-criterion isosurface, density, pressure coefficient with shock isosurface, spanwise velocity, spanwise vorticity, and lift-coefficient history.</figcaption>
</figure>

__Publication:__


|        |  |
|   :-:    | -       |
| <img src='../images/publication/buffet_alleviation.png' align="center" width="200" height="10"> | Rohit Sunil Kanchi, __Sicheng He__, Eirikur Jonsson, Joaquim R. R. A. Martins.  <br><br> [__Buffet Alleviation via Linear Stability Adjoint__](https://arxiv.org/abs/2605.04884)  <br><br> _AIAA AVIATION Forum_ (2026). **2026 AIAA MDO Best Student Paper Runner-Up.**|


## 1. Structured representations of nonlinear dynamics

<figure class="lab-figure">
  <img src="../images/publication/wing_tsm_oscillation.gif" alt="Coupled time-spectral aeroelastic wing oscillation">
  <figcaption>Forced periodic oscillation of a flexible wing computed with our coupled time-spectral aeroelastic solver, capturing the fluid–structure response in the frequency domain at a fraction of the cost of time marching.</figcaption>
</figure>

**How do we build compact, structured representations of nonlinear time-dependent dynamics?**

We develop spectral and frequency-domain frameworks that replace brute-force time marching with structure-exploiting representations of periodic and quasi-periodic behavior.
Our work follows a natural progression: **represent** the motion via time-spectral methods, **generalize** to multi-frequency motion via torus methods, and **characterize stability** of the represented motion via Floquet theory.

Key contributions include the **torus time-spectral method (TTSM)** that lifts governing equations to an extended angular phase space with **spectral convergence**, **spectral Floquet analysis** for orbital stability of periodic systems, **time-spectral resolvent analysis** for frequency response of periodically varying base flows, and the **first fully coupled CFD–FEA time-spectral aeroelastic solver** that captures forced periodic wing oscillations in the frequency domain at a **fraction of the cost** of time marching.

__Publication:__


|        |  |
|   :-:    | -       |
| <img src='../images/publication/torus.png' align="center" width="200" height="10"> | __Sicheng He__, Hang Li, Kivanc Ekici.  <br><br> [__Torus Time-Spectral Method for Quasi-Periodic Problems__](https://arxiv.org/abs/2512.13631)  <br><br> _arXiv preprint_ (2025).|
| <img src='../images/publication/torus_ts_wing.png' align="center" width="200" height="10"> | __Sicheng He__, Rohit Kanchi.  <br><br> __Torus Time-Spectral Method for Three-Dimensional Wing Oscillations with Two Incommensurate Frequencies__  <br><br> _in preparation_.|
| <img src='../images/publication/floquet.png' align="center" width="200" height="10"> | __Sicheng He__, Max Howell, Dan Wilson.  <br><br> __Time-Spectral Method-Based Efficient Floquet Analysis__  <br><br> _in preparation_.|
| <img src='../images/publication/ts_resolvent.png' align="center" width="200" height="10"> | Max Howell, __Sicheng He__.  <br><br> [__Time-Spectral Resolvent Analysis for Periodic Dynamical Systems__](https://arxiv.org/abs/2602.15194)  <br><br> _SIAM Journal on Applied Dynamical Systems (submitted)_ (2026).|
| <img src='../images/publication/wing_tsm_oscillation.gif' align="center" width="200" height="10"> | __Sicheng He__.  <br><br> __Coupled Time-Spectral Aeroelastic Analysis Using High-Fidelity CFD and Finite Element Structural Models__  <br><br> _in preparation_.|


## 2. Operator-theoretic analysis and interpretable reduced coordinates

<figure class="lab-figure">
  <img src="../images/research/uvel_response_mode_top_view.png" alt="Resolvent response mode on NASA CRM wing">
  <figcaption>Velocity resolvent response mode on the NASA Common Research Model wing, computed using our matrix-free resolvent analysis framework.</figcaption>
</figure>

**How do we extract the dominant mechanisms, coordinates, and sensitivities from large-scale nonlinear systems?**

We build modal and operator-based tools to turn simulation data or linearized operators into understanding: what modes matter, what forcing/response structures dominate, and how sensitivities propagate through modal objects.
Critically, our analysis tools are not passive diagnostics—they are made **optimization-ready** through differentiable formulations that connect directly to gradient-based design.

Key contributions include the first **fully matrix-free resolvent analysis** for 3D aerodynamic systems (NASA CRM, **1.8 million cells**), **differentiable resolvent analysis** for flow control optimization, and **differentiable POD** for optimization-compatible modal decompositions and field inversion.

__Publication:__


|        |  |
|   :-:    | -       |
| <img src='../images/publication/uvel_response_mode_top_view.png' align="center" width="200" height="10"> | __Sicheng He__, Rohit Kanchi.  <br><br> __Matrix-Free Resolvent Analysis for Large-Scale Aerodynamic Systems__  <br><br> _in preparation_.|
| <img src='../images/publication/resolvent_opt.png' align="center" width="200" height="10"> | __Sicheng He__, Shugo Kaneko, Daning Huang, Chi-An Yeh, Joaquim R. R. A. Martins.  <br><br> __Large-Scale Flow Control Performance Optimization via Differentiable Resolvent Analysis__  <br><br> _in preparation_.|
| <img src='../images/publication/pod_overview.png' align="center" width="200" height="10"> | Rohit Sunil Kanchi, __Sicheng He__.  <br><br> [__Modal-Centric Field Inversion via Differentiable Proper Orthogonal Decomposition__](https://arxiv.org/abs/2601.14858)  <br><br> _Journal of Computational Physics (major revision submitted)_ (2026).|


## 3. Optimization, control, and learning of dynamical systems

**How do we control, optimize, and learn within structured dynamical representations?**

Once dynamics are represented and interpreted, we ask: how do we modify them—suppress instability, improve performance, learn closures, and design systems with dynamics as first-class constraints?
We combine adjoint methods, multidisciplinary optimization, and scientific machine learning to design, stabilize, and infer complex engineering systems governed by multiscale dynamics.

Key contributions include adjoint-based **stability-constrained design optimization**, **Hopf-bifurcation instability suppression** via the first Lyapunov coefficient, adjoint-based **control co-design**, including **co-design of legged robots** with parallel elasticity, a **fundamental** reverse algorithmic differentiation method for complex analytic functions yielding the **first succinct eigenvalue derivative formula for general complex matrices**, gradient-enhanced **neural network surrogates** for real-time aerodynamic analysis ([Webfoil](http://webfoil.engin.umich.edu/)), the **differentiable Kalman filter** for physics-informed state estimation with **90% error reduction**, and the **UniFoil** dataset of 500,000 airfoil simulations for scientific machine learning.

<figure class="lab-figure">
  <div class="lab-video">
    <iframe width="800" height="450" src="https://www.youtube-nocookie.com/embed/Qr4zfAnQmRc?rel=0" title="SurGE: co-design of legged robots with parallel elasticity" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen loading="lazy"></iframe>
  </div>
  <figcaption>SurGE co-designs the parallel spring of a hopping robot with surrogate gradients from a differentiable dynamics and control pipeline; on hardware it reduces the design objective by 37.65% (IROS 2026, with Yanran Ding's <a href="https://sites.google.com/umich.edu/arcad-lab/">ARCaD Lab</a> at the University of Michigan).</figcaption>
</figure>

<figure class="lab-figure">
  <div class="lab-figure-row">
    <img src="../images/research/baseline.gif" alt="baseline">
    <img src="../images/research/optimized.gif" alt="optimized">
  </div>
  <figcaption>Baseline (left) and optimized (right).</figcaption>
</figure>

__Publication:__


|        |  |
|   :-:    | -       |
| <img src='../images/publication/surge.jpg' align="center" width="200" height="10"> | Yulun Zhuang, Yue Qin, Justin Lu, Zelin Shen, Yichen Wang, __Sicheng He__, Yanran Ding.  <br><br> [__SurGE: Surrogate Gradient-guided Evolution for Co-design of Legged Robots with Parallel Elasticity__](https://arxiv.org/abs/2606.21866)  <br><br> _IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)_ (2026). [[Project page]](https://arcad-lab-um.github.io/surge-codesign/) [[Video]](https://youtu.be/Qr4zfAnQmRc)|
| <img src='../images/publication/score_diffusion.png' align="center" width="200" height="10"> | Minglei Yang, __Sicheng He__.  <br><br> [__Training-Free Score-Based Diffusion for Parameter-Dependent Stochastic Dynamical Systems__](https://doi.org/10.3934/acse.2026005)  <br><br> _Advances in Computational Science and Engineering_ (2026).|
|  | Jianing Chen, Yan Li, __Sicheng He__, Daning Huang.  <br><br> [__Eigenvalue- and Gradient-Aware Optimization for Small-Signal Stability via the Adjoint Method__](https://doi.org/10.1109/TPWRS.2026.3725599)  <br><br> _IEEE Transactions on Power Systems_ (2026).|
| <img src='../images/publication/blade_design.png' align="center" width="200" height="10"> | __Sicheng He__, Shugo Kaneko, Max Howell, Nan Li, Joaquim R. R. A. Martins.  <br><br> [__Efficient Adjoint-based Design Optimization with Optimal Control__](https://www.researchgate.net/publication/398712239_Efficient_Adjoint-based_Design_Optimization_with_Optimal_Control)  <br><br> _Journal of Mechanical Design (accepted)_ (2026).|
| <img src='../images/publication/hydrofoil_flutter_opt.png' align="center" width="200" height="10"> | Galen W. Ng, Shugo Kaneko, Eirikur Jonsson, __Sicheng He__, Joaquim R. R. A. Martins.  <br><br> __Hydroelastic Optimization of Submerged Composite Foils with Flutter and Ventilation Constraints__  <br><br> _Structural and Multidisciplinary Optimization (accepted)_ (2026).|
| <img src='../images/publication/unifoil.png' align="center" width="200" height="10"> | Rohit Sunil Kanchi, Benjamin Melanson, Nithin Somasekharan, Shaowu Pan, __Sicheng He__.  <br><br> [__UniFoil: A Universal Dataset of Airfoils in Transitional and Turbulent Regimes for Subsonic and Transonic Flows__](https://arxiv.org/abs/2505.21124)  <br><br> _NeurIPS Datasets and Benchmarks Track_ (2025).|
| <img src='../images/publication/bif_stability.png' align="center" width="200" height="10"> | __Sicheng He__, Max Howell, Daning Huang, Eirikur Jonsson, Galen W. Ng, Joaquim R. R. A. Martins.  <br><br> [__Adjoint-based Hopf-bifurcation Instability Suppression via First Lyapunov Coefficient__](https://arxiv.org/abs/2511.03840)  <br><br> _AIAA Journal (major revision)_ (2025).|
| <img src='../images/publication/diff_kf.png' align="center" width="200" height="10"> | Yuan Wu, __Sicheng He__.  <br><br> [__DKFNet: Differentiable Kalman Filter for Field Inversion and Machine Learning__](https://arxiv.org/abs/2509.07474)  <br><br> _Journal of Computational Physics (under review)_ (2025).|
| <img src='../images/publication/LST.png' align="center" width="200" height="10"> | __Sicheng He__, Eirikur Jonsson, Jichao Li, Joaquim R. R. A. Martins.  <br><br> [__Adjoint-Based Design Optimization of Stability Constrained Systems__](https://arc.aiaa.org/doi/10.2514/1.J064273)  <br><br> _AIAA Journal_ (2024).|
| <img src='../images/publication/LCO_stability.png' align="center" width="200" height="10"> | __Sicheng He__, Eirikur Jonsson, Joaquim R. R. A. Martins.  <br><br> [__Adjoint-based Limit Cycle Oscillation Instability Sensitivity and Suppression__](https://www.researchgate.net/publication/363581644_Adjoint-based_Limit_Cycle_Oscillation_Instability_Sensitivity_and_Suppression)  <br><br> _Nonlinear dynamics_ (2022).|
| <img src='../images/publication/complex_eigen.png' align="center" width="200" height="10"> | __Sicheng He__, Yayun Shi, Eirikur Jonsson, Joaquim R. R. A. Martins.  <br><br> [__Eigenvalue problem derivatives computation for a complex matrix using the adjoint method__](https://www.researchgate.net/publication/362931690_Eigenvalue_problem_derivatives_computation_for_a_complex_matrix_using_the_adjoint_method)  <br><br> _Mechanical Systems and Signal Processing_ (2023).|
| <img src='../images/publication/eigenXDSM.png' align="center" width="200" height="10"> | __Sicheng He__, Eirikur Jonsson, and Joaquim R. R. A. Martins.  <br><br> [__Derivatives for Eigenvalues and Eigenvectors via Analytic Reverse Algorithmic Differentiation__](https://arc.aiaa.org/doi/abs/10.2514/1.J060726?journalCode=aiaaj)  <br><br> _AIAA Journal_ (2022).|
| <img src='../images/publication/buffet.png' align="center" width="200" height="10"> | Jichao Li, __Sicheng He__, Mengqi Zhang, Joaquim R. R. A. Martins, Boo Cheong Khoo.  <br><br> [__Physics-Based Data-Driven Buffet-Onset Constraint for Aerodynamic Shape Optimization__](https://arc.aiaa.org/doi/10.2514/1.J061519)  <br><br> _AIAA Journal_ (2022).|
| <img src='../images/publication/transonic.png' align="center" width="200" height="10"> | Mohamed Amine Bouhlel, __Sicheng He__, and Joaquim R. R. A. Martins. <br><br> [__Scalable gradient-enhanced artiﬁcial neural networks for airfoil shape design in the subsonic and transonic regimes__](https://link.springer.com/article/10.1007/s00158-020-02488-5)  <br><br> _Structural and Multidisciplinary Optimization_ (2020). (Webfoil)|
| <img src='../images/publication/stream.png' align="center" width="200" height="10"> | Jichao Li, __Sicheng He__, and Joaquim R. R. A. Martins. <br><br> [__Data-driven constraint approach to ensure low-speed performance in transonic aerodynamic shape optimization__](https://www.sciencedirect.com/science/article/pii/S1270963819304912)  <br><br> _Aerospace Science and Technology_ (2019).|


[Past research projects](/past-research/) — aeroelastic optimization, wind turbine MDO, laminar-turbulent transition, structural global optimization.
