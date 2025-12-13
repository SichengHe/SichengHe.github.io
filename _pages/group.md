---
layout: archive
title: "CODES Group"
permalink: /group/
author_profile: false
redirect_from:
  - /group
---

<p style="text-align: center; font-size: 1.1em; color: #666; margin-bottom: 2em;">
<strong>C</strong>omputational <strong>O</strong>ptimization for <strong>D</strong>ynamics and <strong>E</strong>ngineering <strong>S</strong>ystems
</p>

<style>
.team-section {
  margin-bottom: 2em;
}

.team-section h2 {
  border-bottom: 2px solid #52adc8;
  padding-bottom: 0.5em;
  margin-bottom: 1em;
}

.team-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 1.5em;
  margin-bottom: 2em;
}

.team-card {
  background: #fff;
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  padding: 1.5em;
  text-align: center;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  transition: box-shadow 0.3s ease;
}

.team-card:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}

.team-card img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 1em;
  border: 3px solid #52adc8;
}

.team-card h3 {
  margin: 0.5em 0 0.25em 0;
  color: #333;
  font-size: 1.1em;
}

.team-card .position {
  color: #666;
  font-style: italic;
  margin-bottom: 0.5em;
}

.team-card .affiliation {
  color: #888;
  font-size: 0.9em;
  margin-bottom: 0.75em;
}

.team-card .education {
  text-align: left;
  font-size: 0.85em;
  color: #555;
  margin-bottom: 0.75em;
}

.team-card .education ul {
  margin: 0;
  padding-left: 1.2em;
}

.team-card .education li {
  margin-bottom: 0.25em;
}

.team-card .links {
  margin-top: 1em;
}

.team-card .links a {
  display: inline-block;
  margin: 0 0.3em;
  color: #52adc8;
  font-size: 1.2em;
  transition: color 0.2s ease;
}

.team-card .links a:hover {
  color: #3a8aa8;
}

/* PI Card - larger and centered */
.pi-section .team-grid {
  justify-content: center;
}

.pi-section .team-card {
  max-width: 400px;
}

.pi-section .team-card img {
  width: 180px;
  height: 180px;
}

/* Alumni table styling */
.alumni-table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 1em;
}

.alumni-table th, .alumni-table td {
  padding: 0.75em;
  text-align: left;
  border-bottom: 1px solid #e0e0e0;
}

.alumni-table th {
  background: #f5f5f5;
  font-weight: 600;
}

.alumni-table tr:hover {
  background: #fafafa;
}

/* Responsive adjustments */
@media (max-width: 600px) {
  .team-grid {
    grid-template-columns: 1fr;
  }

  .team-card img {
    width: 120px;
    height: 120px;
  }
}
</style>

<!-- Principal Investigator -->
<div class="team-section pi-section">
<h2>Principal Investigator</h2>
<div class="team-grid">
{% for member in site.data.team.principal_investigator %}
<div class="team-card">
  <img src="{{ member.photo | relative_url }}" alt="{{ member.name }}" onerror="this.src='{{ '/images/bio-photo.jpg' | relative_url }}'">
  <h3>{{ member.name }}</h3>
  <div class="position">{{ member.position }}</div>
  <div class="affiliation">{{ member.affiliation }}</div>
  {% if member.education %}
  <div class="education">
    <ul>
    {% for edu in member.education %}
      <li>{{ edu.degree }} {{ edu.field }}, {{ edu.institution }}{% if edu.year %}, {{ edu.year }}{% endif %}</li>
    {% endfor %}
    </ul>
  </div>
  {% endif %}
  <div class="links">
    {% if member.links.google_scholar %}<a href="{{ member.links.google_scholar }}" title="Google Scholar" target="_blank"><i class="ai ai-google-scholar"></i></a>{% endif %}
    {% if member.links.researchgate %}<a href="{{ member.links.researchgate }}" title="ResearchGate" target="_blank"><i class="ai ai-researchgate"></i></a>{% endif %}
    {% if member.links.github %}<a href="{{ member.links.github }}" title="GitHub" target="_blank"><i class="fab fa-github"></i></a>{% endif %}
    {% if member.links.linkedin %}<a href="{{ member.links.linkedin }}" title="LinkedIn" target="_blank"><i class="fab fa-linkedin"></i></a>{% endif %}
    {% if member.links.orcid %}<a href="{{ member.links.orcid }}" title="ORCID" target="_blank"><i class="ai ai-orcid"></i></a>{% endif %}
    {% if member.links.email %}<a href="mailto:{{ member.links.email }}" title="Email"><i class="fas fa-envelope"></i></a>{% endif %}
  </div>
</div>
{% endfor %}
</div>
</div>

<!-- PhD Students -->
{% if site.data.team.phd_students.size > 0 %}
<div class="team-section">
<h2>Ph.D. Students</h2>
<div class="team-grid">
{% for member in site.data.team.phd_students %}
<div class="team-card">
  <img src="{{ member.photo | relative_url }}" alt="{{ member.name }}" onerror="this.src='{{ '/images/bio-photo.jpg' | relative_url }}'">
  <h3>{{ member.name }}</h3>
  <div class="position">{{ member.position }}</div>
  <div class="affiliation">{{ member.affiliation }}</div>
  {% if member.education %}
  <div class="education">
    <ul>
    {% for edu in member.education %}
      <li>{{ edu.degree }} {{ edu.field }}, {{ edu.institution }}{% if edu.year %}, {{ edu.year }}{% endif %}</li>
    {% endfor %}
    </ul>
  </div>
  {% endif %}
  <div class="links">
    {% if member.links.google_scholar %}<a href="{{ member.links.google_scholar }}" title="Google Scholar" target="_blank"><i class="ai ai-google-scholar"></i></a>{% endif %}
    {% if member.links.researchgate %}<a href="{{ member.links.researchgate }}" title="ResearchGate" target="_blank"><i class="ai ai-researchgate"></i></a>{% endif %}
    {% if member.links.github %}<a href="{{ member.links.github }}" title="GitHub" target="_blank"><i class="fab fa-github"></i></a>{% endif %}
    {% if member.links.linkedin %}<a href="{{ member.links.linkedin }}" title="LinkedIn" target="_blank"><i class="fab fa-linkedin"></i></a>{% endif %}
    {% if member.links.orcid %}<a href="{{ member.links.orcid }}" title="ORCID" target="_blank"><i class="ai ai-orcid"></i></a>{% endif %}
    {% if member.links.email %}<a href="mailto:{{ member.links.email }}" title="Email"><i class="fas fa-envelope"></i></a>{% endif %}
  </div>
</div>
{% endfor %}
</div>
</div>
{% endif %}

<!-- Masters Students -->
{% if site.data.team.masters_students.size > 0 %}
<div class="team-section">
<h2>Master's Students</h2>
<div class="team-grid">
{% for member in site.data.team.masters_students %}
<div class="team-card">
  <img src="{{ member.photo | relative_url }}" alt="{{ member.name }}" onerror="this.src='{{ '/images/bio-photo.jpg' | relative_url }}'">
  <h3>{{ member.name }}</h3>
  <div class="position">{{ member.position }}</div>
  <div class="affiliation">{{ member.affiliation }}</div>
  {% if member.education %}
  <div class="education">
    <ul>
    {% for edu in member.education %}
      <li>{{ edu.degree }} {{ edu.field }}, {{ edu.institution }}{% if edu.year %}, {{ edu.year }}{% endif %}</li>
    {% endfor %}
    </ul>
  </div>
  {% endif %}
  <div class="links">
    {% if member.links.google_scholar %}<a href="{{ member.links.google_scholar }}" title="Google Scholar" target="_blank"><i class="ai ai-google-scholar"></i></a>{% endif %}
    {% if member.links.researchgate %}<a href="{{ member.links.researchgate }}" title="ResearchGate" target="_blank"><i class="ai ai-researchgate"></i></a>{% endif %}
    {% if member.links.github %}<a href="{{ member.links.github }}" title="GitHub" target="_blank"><i class="fab fa-github"></i></a>{% endif %}
    {% if member.links.linkedin %}<a href="{{ member.links.linkedin }}" title="LinkedIn" target="_blank"><i class="fab fa-linkedin"></i></a>{% endif %}
    {% if member.links.orcid %}<a href="{{ member.links.orcid }}" title="ORCID" target="_blank"><i class="ai ai-orcid"></i></a>{% endif %}
    {% if member.links.email %}<a href="mailto:{{ member.links.email }}" title="Email"><i class="fas fa-envelope"></i></a>{% endif %}
  </div>
</div>
{% endfor %}
</div>
</div>
{% endif %}

<!-- Undergraduate Students -->
{% if site.data.team.undergraduate_students.size > 0 %}
<div class="team-section">
<h2>Undergraduate Students</h2>
<div class="team-grid">
{% for member in site.data.team.undergraduate_students %}
<div class="team-card">
  <img src="{{ member.photo | relative_url }}" alt="{{ member.name }}" onerror="this.src='{{ '/images/bio-photo.jpg' | relative_url }}'">
  <h3>{{ member.name }}</h3>
  <div class="position">{{ member.position }}</div>
  <div class="affiliation">{{ member.affiliation }}</div>
  {% if member.education %}
  <div class="education">
    <ul>
    {% for edu in member.education %}
      <li>{{ edu.degree }} {{ edu.field }}, {{ edu.institution }}{% if edu.year %}, {{ edu.year }}{% endif %}</li>
    {% endfor %}
    </ul>
  </div>
  {% endif %}
  <div class="links">
    {% if member.links.google_scholar %}<a href="{{ member.links.google_scholar }}" title="Google Scholar" target="_blank"><i class="ai ai-google-scholar"></i></a>{% endif %}
    {% if member.links.researchgate %}<a href="{{ member.links.researchgate }}" title="ResearchGate" target="_blank"><i class="ai ai-researchgate"></i></a>{% endif %}
    {% if member.links.github %}<a href="{{ member.links.github }}" title="GitHub" target="_blank"><i class="fab fa-github"></i></a>{% endif %}
    {% if member.links.linkedin %}<a href="{{ member.links.linkedin }}" title="LinkedIn" target="_blank"><i class="fab fa-linkedin"></i></a>{% endif %}
    {% if member.links.orcid %}<a href="{{ member.links.orcid }}" title="ORCID" target="_blank"><i class="ai ai-orcid"></i></a>{% endif %}
    {% if member.links.email %}<a href="mailto:{{ member.links.email }}" title="Email"><i class="fas fa-envelope"></i></a>{% endif %}
  </div>
</div>
{% endfor %}
</div>
</div>
{% endif %}

<!-- Alumni -->
{% if site.data.team.alumni.size > 0 %}
<div class="team-section">
<h2>Alumni</h2>
<table class="alumni-table">
  <thead>
    <tr>
      <th>Name</th>
      <th>Degree</th>
      <th>Year</th>
      <th>First Position</th>
      <th>Current Position</th>
    </tr>
  </thead>
  <tbody>
  {% for alum in site.data.team.alumni %}
    <tr>
      <td>{{ alum.name }}</td>
      <td>{{ alum.degree }}</td>
      <td>{{ alum.graduation_year }}</td>
      <td>{{ alum.first_position }}</td>
      <td>{{ alum.current_position }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
</div>
{% endif %}
