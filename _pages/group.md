---
layout: page
permalink: /group/
title: Group
description: Meet our group.
nav: true
nav_order: 3
---

{% assign group_order = "Postdocs|PhD Students|MS Students|Undergraduates|Visitors|Alumni" | split: "|" %}

{% for g in group_order %}
  {% assign members = site.data.people | where: "group", g | sort: "order" %}
  {% if members.size > 0 %}
  ### {{ g }}

  <div class="people-grid">
    {% for p in members %}

      <div class="person-card">
        <div class="person-headshot">
          {% if p.headshot %}
            <img src="{{ p.headshot }}" alt="{{ p.name }} headshot" loading="lazy">
          {% else %}
            <div class="placeholder" aria-hidden="true">No Photo</div>
          {% endif %}
        </div>

        <div class="person-body">
          <div class="person-name">
            {% if p.website %}
              <a href="{{ p.website }}" target="_blank" rel="noopener">{{ p.name }}</a>
            {% else %}
              {{ p.name }}
            {% endif %}
          </div>

          {% if p.role %}
            <div class="person-role">{{ p.role }}</div>
          {% endif %}

          {% if p.bio %}
            <div class="person-bio">{{ p.bio }}</div>
          {% endif %}

          <div class="person-links">
            {% if p.website %}
              <a href="{{ p.website }}" target="_blank" rel="noopener" aria-label="{{ p.name }} website">🌐</a>
            {% endif %}
            {% if p.linkedin %}
              <a href="{{ p.linkedin }}" target="_blank" rel="noopener" aria-label="{{ p.name }} LinkedIn">in</a>
            {% endif %}
            {% if p.scholar %}
              <a href="{{ p.scholar }}" target="_blank" rel="noopener" aria-label="{{ p.name }} Google Scholar">G</a>
            {% endif %}
            {% if p.github %}
              <a href="{{ p.github }}" target="_blank" rel="noopener" aria-label="{{ p.name }} GitHub">GH</a>
            {% endif %}
            {% if p.email %}
              <a href="mailto:{{ p.email }}" aria-label="Email {{ p.name }}">✉️</a>
            {% endif %}
          </div>
        </div>
      </div>

    {% endfor %}
  </div>

  {% endif %}
{% endfor %}

<style>
/* Minimal, Folio-friendly styling */
.people-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
  grid-gap: 1.25rem;
  margin-top: 0.5rem;
}
.person-card {
  display: grid;
  grid-template-rows: auto 1fr;
  gap: 0.6rem;
  padding: 1rem;
  border: 1px solid var(--border, #e5e7eb);
  border-radius: 0.75rem;
  background: var(--card, #fff);
}
.person-headshot img {
  width: 100%;
  height: 240px;
  object-fit: cover;
  border-radius: 0.5rem;
}
.person-headshot .placeholder {
  width: 100%;
  height: 240px;
  display: grid;
  place-items: center;
  background: #f3f4f6;
  color: #6b7280;
  border-radius: 0.5rem;
  font-size: 0.9rem;
}
.person-name {
  font-weight: 600;
  font-size: 1.05rem;
  line-height: 1.2;
  margin-bottom: 0.15rem;
}
.person-role {
  color: #6b7280;
  font-size: 0.95rem;
  margin-bottom: 0.4rem;
}
.person-bio {
  font-size: 0.95rem;
  line-height: 1.4;
  margin-bottom: 0.5rem;
}
.person-links a {
  display: inline-block;
  margin-right: 0.5rem;
  text-decoration: none;
  font-weight: 600;
  border-bottom: 1px solid transparent;
}
.person-links a:hover { border-color: currentColor; }
</style>

