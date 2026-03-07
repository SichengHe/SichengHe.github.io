title: "Differentiable singular value decomposition (SVD)"
collection: publications
permalink: /publication/2025-06-16-diffsvd-kanchi-he
excerpt: "Introduces adjoint- and reverse automatic differentiation-based algorithms that deliver machine-precision singular-value derivatives without scaling with the number of design variables."
date: 2025-06-16
venue: 'Mechanical Systems and Signal Processing'
paperurl: '/files/diffsvd_Kanchi_and_He.pdf'
citation: 'Kanchi, Rohit Sunil, and Sicheng He. (2025). &quot;Differentiable singular value decomposition (SVD).&quot; <i>Mechanical Systems and Signal Processing</i>, 237:112817.'
---
We present two adjoint formulations for differentiating the singular value decomposition of general complex matrices—one leveraging the Gram matrices that arise in the eigenvalue/SVD connection and the other based on the symmetric embedding approach. Both variants deliver machine-precision derivatives while keeping the cost independent of the number of design variables, which makes them suitable for large-scale gradient-based optimization workflows.

To complement the adjoint approaches we also derive a reverse automatic differentiation (RAD) formula that provides singular-value sensitivities for complex inputs without storing every singular vector. The adjoint and RAD methods are validated against finite-difference benchmarks for square and rectangular matrices, and we demonstrate scalability by differentiating the snapshot matrix from the Johns Hopkins turbulence database POD case of laminar–turbulent transition over a flat plate.

[Download paper here](/files/diffsvd_Kanchi_and_He.pdf)

Recommended citation: Kanchi, Rohit Sunil, and Sicheng He. "Differentiable singular value decomposition (SVD)." <i>Mechanical Systems and Signal Processing</i> 237 (2025): 112817.
