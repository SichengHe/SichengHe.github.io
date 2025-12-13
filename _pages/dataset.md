---
layout: archive
title: "Dataset"
permalink: /dataset/
author_profile: false
---

<style>
.dataset-card {
  background: #fff;
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  padding: 1.5em;
  margin-bottom: 1.5em;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  border-left: 4px solid #ff8200;
}

.dataset-card h2 {
  color: #ff8200;
  margin-top: 0;
  margin-bottom: 0.5em;
}

.dataset-card .subtitle {
  color: #666;
  font-style: italic;
  margin-bottom: 1em;
}

.dataset-card .description {
  color: #444;
  margin-bottom: 1em;
  line-height: 1.6;
}

.dataset-card .stats {
  display: flex;
  flex-wrap: wrap;
  gap: 1em;
  margin-bottom: 1em;
  padding: 1em;
  background: #f9f9f9;
  border-radius: 4px;
}

.dataset-card .stat-item {
  flex: 1;
  min-width: 150px;
  text-align: center;
}

.dataset-card .stat-number {
  font-size: 1.5em;
  font-weight: bold;
  color: #ff8200;
}

.dataset-card .stat-label {
  font-size: 0.85em;
  color: #666;
}

.dataset-card .details {
  margin-bottom: 1em;
}

.dataset-card .details ul {
  margin: 0.5em 0;
  padding-left: 1.5em;
}

.dataset-card .details li {
  margin-bottom: 0.3em;
  color: #555;
}

.dataset-card .citation {
  background: #fff8f0;
  border: 1px solid #ffe0c0;
  border-radius: 4px;
  padding: 1em;
  margin-bottom: 1em;
  font-size: 0.9em;
}

.dataset-card .citation-title {
  font-weight: bold;
  color: #333;
  margin-bottom: 0.5em;
}

.dataset-card .links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5em;
}

.dataset-card .links a {
  display: inline-block;
  background: #ff8200;
  color: white !important;
  padding: 0.5em 1em;
  border-radius: 4px;
  text-decoration: none !important;
  font-size: 0.9em;
  transition: background 0.2s;
}

.dataset-card .links a:hover {
  background: #e07000;
}

.dataset-card .links a i {
  margin-right: 0.3em;
}
</style>

<div class="dataset-card">
  <h2>UniFoil</h2>
  <div class="subtitle">A Universal Dataset of Airfoils in Transitional and Turbulent Regimes for Subsonic and Transonic Flows</div>

  <div class="description">
    <p>UniFoil is a comprehensive dataset comprising <strong>500,000 computational simulations</strong> of 2D airfoils, designed for machine learning applications in aerodynamic analysis and design optimization. The dataset covers multiple flow regimes including subsonic and transonic conditions.</p>
  </div>

  <div class="stats">
    <div class="stat-item">
      <div class="stat-number">500K</div>
      <div class="stat-label">Total Simulations</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">400K</div>
      <div class="stat-label">Fully Turbulent (FT)</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">50K</div>
      <div class="stat-label">NLF Turbulent</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">50K</div>
      <div class="stat-label">NLF Transitional</div>
    </div>
  </div>

  <div class="details">
    <strong>Dataset includes:</strong>
    <ul>
      <li>400,000 fully-turbulent (FT) airfoil simulations</li>
      <li>50,000 natural laminar flow (NLF) simulations in fully turbulent conditions</li>
      <li>50,000 NLF simulations in transitional flow regimes</li>
    </ul>
  </div>

  <div class="citation">
    <div class="citation-title">Citation</div>
    <p>Kanchi, Melanson, Somasekharan, Pan, and He. "UniFoil: A Universal Dataset of Airfoils." Harvard Dataverse, 2025. DOI: 10.7910/DVN/VQGWC4</p>
    <p>Paper: <a href="https://arxiv.org/abs/2505.21124" target="_blank">arXiv:2505.21124</a></p>
  </div>

  <div class="links">
    <a href="https://github.com/rohitroxkp7/UniFoil" target="_blank"><i class="fab fa-github"></i> GitHub</a>
    <a href="https://doi.org/10.7910/DVN/VQGWC4" target="_blank"><i class="fas fa-database"></i> Harvard Dataverse</a>
    <a href="https://arxiv.org/abs/2505.21124" target="_blank"><i class="fas fa-file-alt"></i> Paper</a>
    <a href="https://unifoildocs.readthedocs.io" target="_blank"><i class="fas fa-book"></i> Documentation</a>
  </div>
</div>
