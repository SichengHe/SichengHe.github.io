---
permalink: /
title: " "
excerpt: "Extreme-Condition Dynamics & Design Lab"
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

<style>
/* Hero Section */
.hero-section {
  background: linear-gradient(135deg, #ff8200 0%, #e07000 100%);
  color: white;
  padding: 3em 2em;
  margin: -1em -1em 2em -1em;
  text-align: center;
}

.hero-section h1 {
  font-size: 2.8em;
  margin: 0 0 0.25em 0;
  font-weight: 700;
}

.hero-section .tagline {
  font-size: 1.3em;
  opacity: 0.95;
  max-width: 700px;
  margin: 0 auto;
}

/* Main Layout */
.main-content {
  max-width: 1100px;
  margin: 0 auto;
}

.content-row {
  display: flex;
  gap: 3em;
  margin-bottom: 2.5em;
}

.content-row.reverse {
  flex-direction: row-reverse;
}

@media (max-width: 768px) {
  .content-row, .content-row.reverse {
    flex-direction: column;
  }
}

/* Profile Section */
.profile-section {
  flex: 0 0 280px;
}

.profile-card {
  text-align: center;
}

.profile-card img {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #ff8200;
  margin-bottom: 1em;
}

.profile-card h3 {
  margin: 0 0 0.25em 0;
  font-size: 1.4em;
  color: #333;
}

.profile-card .title {
  color: #666;
  font-size: 1em;
  margin-bottom: 0.5em;
}

.profile-card .affiliation {
  font-size: 0.9em;
  color: #888;
  margin-bottom: 1em;
}

.profile-card .social-links {
  display: flex;
  justify-content: center;
  gap: 0.75em;
  flex-wrap: wrap;
}

.profile-card .social-links a {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 36px;
  height: 36px;
  background: #f0f0f0;
  border-radius: 50%;
  color: #555;
  font-size: 1.1em;
  transition: all 0.2s;
  text-decoration: none;
}

.profile-card .social-links a:hover {
  background: #ff8200;
  color: white;
}

.contact-info {
  margin-top: 1.5em;
  text-align: left;
  font-size: 0.9em;
  color: #555;
}

.contact-info p {
  margin: 0.4em 0;
}

.contact-info i {
  width: 20px;
  color: #ff8200;
}

/* Welcome Section */
.welcome-section {
  flex: 1;
}

.welcome-section h2 {
  color: #ff8200;
  font-size: 1.6em;
  margin-top: 0;
  margin-bottom: 0.75em;
  border-bottom: 2px solid #ff8200;
  padding-bottom: 0.5em;
}

.welcome-section p {
  font-size: 1.05em;
  line-height: 1.7;
  color: #444;
}

/* News Section */
.news-section {
  flex: 1;
}

.news-section h2 {
  color: #ff8200;
  font-size: 1.6em;
  margin-top: 0;
  margin-bottom: 0.75em;
  border-bottom: 2px solid #ff8200;
  padding-bottom: 0.5em;
}

.news-item {
  display: flex;
  gap: 1em;
  padding: 0.6em 0;
  border-bottom: none;
}

.news-item:last-child {
  border-bottom: none;
}

.news-date {
  flex: 0 0 70px;
  font-size: 0.9em;
  color: #b31b1b;
  font-weight: 600;
}

.news-content {
  flex: 1;
  font-size: 0.95em;
  color: #333;
  line-height: 1.5;
}

.news-content a {
  color: #b31b1b;
}

.news-content strong {
  color: #333;
}

/* Openings Section */
.openings-section {
  flex: 0 0 320px;
}

.openings-box {
  background: #fff8f0;
  border: 2px solid #ff8200;
  border-radius: 8px;
  padding: 1.5em;
}

.openings-box h2 {
  color: #ff8200;
  font-size: 1.3em;
  margin: 0 0 1em 0;
}

.openings-box p {
  font-size: 0.95em;
  color: #444;
  margin: 0.75em 0;
}

.openings-box .highlight {
  background: #ff8200;
  color: white;
  padding: 0.75em 1em;
  border-radius: 4px;
  font-weight: 500;
  margin-bottom: 1em;
}

.btn-primary {
  display: inline-block;
  background: #ff8200;
  color: white !important;
  padding: 0.6em 1.2em;
  border-radius: 4px;
  text-decoration: none !important;
  font-weight: 500;
  margin-top: 0.5em;
  transition: background 0.2s;
}

.btn-primary:hover {
  background: #e07000;
}

/* Research Highlights */
.research-section h2 {
  color: #ff8200;
  font-size: 1.6em;
  margin-bottom: 1em;
  border-bottom: 2px solid #ff8200;
  padding-bottom: 0.5em;
}

.research-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5em;
}

.research-card {
  background: #f9f9f9;
  padding: 1.25em;
  border-radius: 6px;
  border-left: 4px solid #ff8200;
}

.research-card h4 {
  margin: 0 0 0.5em 0;
  color: #333;
  font-size: 1.05em;
}

.research-card ul {
  margin: 0;
  padding-left: 1.2em;
  font-size: 0.9em;
  color: #555;
}

.research-card li {
  margin-bottom: 0.3em;
}

/* Footer */
.site-footer {
  margin-top: 3em;
  padding-top: 1.5em;
  border-top: 1px solid #ddd;
  text-align: center;
  font-size: 0.85em;
  color: #888;
}

.visitor-map {
  margin-top: 1em;
}

.visitor-map img {
  max-width: 200px;
  opacity: 0.8;
}
</style>

<!-- Hero Section -->
<div class="hero-section">
  <h1>XD<sup>2</sup> Lab</h1>
  <p class="tagline">Extreme-Condition Dynamics &amp; Design Lab — designing systems that operate near their instability limits</p>
</div>

<div class="main-content">

<!-- Row 1: Profile + Welcome -->
<div class="content-row">
  <div class="profile-section">
    <div class="profile-card">
      <img src="/images/sicheng_utk.png" alt="Sicheng He">
      <h3>Sicheng He</h3>
      <div class="title">Assistant Professor</div>
      <div class="affiliation">
        Mechanical and Aerospace Engineering<br>
        University of Tennessee, Knoxville
      </div>
      <div class="social-links">
        <a href="https://scholar.google.com/citations?user=qS7fVDAAAAAJ&hl=en" title="Google Scholar" target="_blank"><i class="fas fa-graduation-cap"></i></a>
        <a href="https://github.com/SichengHe" title="GitHub" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://www.researchgate.net/profile/Sicheng-He" title="ResearchGate" target="_blank"><i class="fab fa-researchgate"></i></a>
        <a href="https://orcid.org/0000-0003-1307-4909" title="ORCID" target="_blank"><i class="fab fa-orcid"></i></a>
      </div>
      <div class="contact-info">
        <p><i class="fas fa-envelope"></i> sicheng@utk.edu</p>
        <p><i class="fas fa-building"></i> Dougherty Engineering Bldg</p>
        <p><i class="fas fa-map-marker-alt"></i> Knoxville, TN 37996</p>
      </div>
    </div>
  </div>

  <div class="welcome-section">
    <h2>Welcome</h2>
    <div style="background: #fff8f0; border-left: 4px solid #ff8200; padding: 0.75em 1em; margin-bottom: 1em; font-style: italic; color: #333;">
      <strong style="font-style: normal;">Our mission:</strong> To develop structured and differentiable representations of complex dynamical systems that enable scalable analysis, physical insight, and optimal design.
    </div>
    <p>
      The <strong>XD<sup>2</sup> Lab</strong> develops mathematical and computational frameworks to <strong>represent</strong>, <strong>interpret</strong>, and <strong>optimize</strong> complex nonlinear dynamical systems — with emphasis on engineering systems that operate near their instability limits.
    </p>
    <p>
      <a href="/research/" class="btn-primary">Explore Our Research</a>
      <a href="/group/" class="btn-primary" style="margin-left: 0.5em;">Meet the Team</a>
    </p>
  </div>
</div>

<!-- Row 2: News + Openings -->
<div class="content-row">
  <div class="news-section">
    <h2>Latest News</h2>
    <div class="news-item">
      <div class="news-date">Jul 2026</div>
      <div class="news-content"><i class="fas fa-file-alt" style="color: #ff8200;"></i> Rohit Kanchi to present at the prestigious <a href="https://www.nas.nasa.gov/pubs/ams.html" target="_blank"><strong>NASA Ames Applied Modeling &amp; Simulation Seminar</strong></a> on July 2.</div>
    </div>
    <div class="news-item">
      <div class="news-date">Jun 2026</div>
      <div class="news-content"><i class="fas fa-file-alt" style="color: #ff8200;"></i> Paper <em>&ldquo;SurGE: Surrogate Gradient-guided Evolution for Co-design of Legged Robots with Parallel Elasticity&rdquo;</em> accepted at <strong>IROS 2026</strong> &mdash; led by <a href="https://silvery107.github.io" target="_blank">Yulun Zhuang</a> and <a href="https://sites.google.com/view/yanranding/home" target="_blank">Yanran Ding</a> (UMich).</div>
    </div>
    <div class="news-item">
      <div class="news-date">Jun 2026</div>
      <div class="news-content"><i class="fas fa-trophy" style="color: #ff8200;"></i> Rohit Kanchi wins <a href="https://www.linkedin.com/feed/update/urn:li:ugcPost:7471734366985973760/" target="_blank"><strong>2026 AIAA Aviation MDO Best Student Paper Runner-Up</strong></a> ($1,000) &mdash; <a href="https://arxiv.org/abs/2605.04884" target="_blank">paper</a>.</div>
    </div>
    <div class="news-item">
      <div class="news-date">Dec 2025</div>
      <div class="news-content"><i class="fas fa-file-alt" style="color: #ff8200;"></i> Rohit Kanchi and Ben Melanson presenting at <strong>NeurIPS 2025</strong>!</div>
    </div>
    <div class="news-item">
      <div class="news-date">Jul 2025</div>
      <div class="news-content"><i class="fas fa-seedling" style="color: #ff8200;"></i> Seed grant from <a href="https://research.utk.edu/aitn/" target="_blank">UTK AI Tennessee Initiative</a> for AI research led by <a href="https://ne.utk.edu/people/vladimir-sobes/" target="_blank">Vladimir Sobes</a> ($50K total, $25K share).</div>
    </div>
    <div class="news-item">
      <div class="news-date">Dec 2024</div>
      <div class="news-content">New lab website launched!</div>
    </div>
    <div class="news-item">
      <div class="news-date">Aug 2023</div>
      <div class="news-content">Prof. He joins UTK MABE as Assistant Professor</div>
    </div>
    <!-- Add more news items as needed -->
  </div>

  <div class="openings-section">
    <div class="openings-box">
      <h2>Open Positions</h2>
      <div class="highlight">Ph.D. positions available!</div>
      <p>We are looking for motivated students interested in MDO, computational physics, scientific computing, and fluid mechanics.</p>
      <p>Graduate students from MABE, EECS, ISE, and applied math at UTK are welcome to reach out.</p>
      <a href="/opening/" class="btn-primary">View Details</a>
    </div>
  </div>
</div>

<!-- Research Highlights -->
<div class="research-section">
  <h2>Research Areas</h2>
  <div class="research-grid">
    <div class="research-card">
      <h4>Structured Representations</h4>
      <ul>
        <li>Time-spectral methods</li>
        <li>Torus methods for quasi-periodic dynamics</li>
        <li>Floquet stability theory</li>
      </ul>
    </div>
    <div class="research-card">
      <h4>Operator-Theoretic Analysis</h4>
      <ul>
        <li>Resolvent analysis</li>
        <li>Differentiable modal decompositions</li>
        <li>Optimization-compatible reduced coordinates</li>
      </ul>
    </div>
    <div class="research-card">
      <h4>Optimization, Control & Learning</h4>
      <ul>
        <li>Adjoint-based stability optimization</li>
        <li>Multidisciplinary design optimization</li>
        <li>Scientific ML for inference and design</li>
      </ul>
    </div>
  </div>
</div>

</div>

<div class="site-footer">
  <p>XD<sup>2</sup> Lab &bull; University of Tennessee, Knoxville &bull; Department of MAE</p>
  <div class="visitor-map">
    <a href="http://www.clustrmaps.com/map/Sichenghe.github.io" title="Visit tracker"><img src="//www.clustrmaps.com/map_v2.png?d=_FCUdA8m1kkps-ZJKEs1uZLeMOm04rrtG03Kyii-QKw" /></a>
  </div>
</div>
