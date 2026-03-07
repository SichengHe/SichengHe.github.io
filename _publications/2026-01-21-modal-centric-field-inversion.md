---
title: "Modal-Centric Field Inversion via Differentiable Proper Orthogonal Decomposition"
collection: publications
permalink: /publication/2026-01-21-modal-centric-field-inversion
excerpt: "Formulates modal-centric field inversion that matches dominant POD modes instead of raw fields and introduces an adjoint-based differentiable POD operator for scalable inverse design."
date: 2026-01-21
venue: 'Journal of Computational Physics (preprint)'
paperurl: '/files/mcfi_paper.pdf'
citation: 'Kanchi, Rohit Sunil, and Sicheng He. (2026). &quot;Modal-Centric Field Inversion via Differentiable Proper Orthogonal Decomposition.&quot; <i>Journal of Computational Physics</i> (under review). arXiv:2601.14858.'
---
We present **modal-centric field inversion (MCFI)**, a framework that solves PDE-constrained inverse problems by matching reduced-order structures rather than full spatio-temporal fields. MCFI operates in the space of dominant proper orthogonal decomposition (POD) modes, which dramatically lowers the objective dimension, regularizes the optimization, and focuses the inversion on physically meaningful flow features.

To enable gradient-based optimization in modal space, we derive a differentiable POD operator whose adjoint formulation evaluates sensitivities of eigenvalues and modes with cost independent of the number of model parameters. We demonstrate MCFI on 1D and 2D modified viscous Burgers problems, recovering spatially varying coefficients that reproduce target dynamics while cutting computational effort relative to finite differences. The approach lays the groundwork for scalable inverse design, closure calibration, and system identification in high-dimensional unsteady flows.

[Download paper here](/files/mcfi_paper.pdf)

Recommended citation: Kanchi, Rohit Sunil, and Sicheng He. "Modal-Centric Field Inversion via Differentiable Proper Orthogonal Decomposition." *Journal of Computational Physics* (preprint), arXiv:2601.14858, 2026.
