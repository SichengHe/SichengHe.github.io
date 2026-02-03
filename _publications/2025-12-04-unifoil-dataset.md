---
title: "UniFoil: A Universal Dataset of Airfoils in Transitional and Turbulent Regimes for Subsonic and Transonic Flows"
collection: publications
permalink: /publication/2025-12-04-unifoil-dataset
excerpt: "Announces UniFoil, a 500k-sample RANS dataset spanning laminar–turbulent transition through fully turbulent subsonic and transonic regimes to accelerate ML research on realistic aerodynamic flows."
date: 2025-12-04
venue: 'NeurIPS Conference (Dataset and Benchmark Track)'
paperurl: '/files/UniFoil_paper.pdf'
citation: 'Kanchi, Rohit Sunil, Benjamin Melanson, Nithin Somasekharan, Shaowu Pan, and Sicheng He. (2025). &quot;UniFoil: A Universal Dataset of Airfoils in Transitional and Turbulent Regimes for Subsonic and Transonic Flows.&quot; <i>NeurIPS Dataset and Benchmark Track</i>, October 2025. arXiv:2505.21124.'
---
We introduce **UniFoil**, the largest public dataset of airfoils simulated with Reynolds-averaged Navier–Stokes (RANS) models across transitional and turbulent flow regimes. The dataset couples an e<sup>N</sup>-based transition prediction method with the Spalart–Allmaras turbulence model and provides more than 500,000 samples covering wide ranges of Reynolds and Mach numbers, angles of attack, and airfoil geometries from natural laminar flow and fully turbulent families. UniFoil explicitly captures nonlinear physics such as laminar–turbulent transition and shock-induced gradients that are absent in most existing aerodynamic ML corpora.

To support scientific machine learning, each sample includes consistent geometry, field, and coefficient data suitable for training surrogate models that must achieve ~1% drag accuracy in multidisciplinary design settings. We demonstrate how the dataset enables benchmarking of modern surrogate architectures and accelerates research on data-driven transition modeling for aerospace, wind energy, and marine applications.

[Download paper here](/files/UniFoil_paper.pdf)

Recommended citation: Kanchi, Rohit Sunil, Benjamin Melanson, Nithin Somasekharan, Shaowu Pan, and Sicheng He. "UniFoil: A Universal Dataset of Airfoils in Transitional and Turbulent Regimes for Subsonic and Transonic Flows." *NeurIPS Dataset and Benchmark Track*, 2025. arXiv:2505.21124.
