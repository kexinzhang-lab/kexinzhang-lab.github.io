---
layout: page
title: research
permalink: /research/
description: Computational imaging and discovery, from molecules to cells.
nav: true
nav_order: 1
---

<div class="research-page">
  <div class="research-intro">
    <h2>From noisy images to molecular discovery</h2>
    <p>We combine physics-based modeling and AI to detect molecules and characterize their structural states directly from cellular cryo-EM/ET data. Our ultimate goal is to understand how the structures of molecular machines relate to their functions in cells, and to use these insights to guide the design of more effective therapeutics.</p>
  </div>

  <nav class="research-index" aria-label="Research projects">
    <span class="research-eyebrow">Explore our projects</span>
    <ol>
      {% for item in site.data.research %}
        <li><a href="#{{ item.id }}">{{ item.short_title }}</a></li>
      {% endfor %}
    </ol>
  </nav>

  <div class="research-projects">
    {% for item in site.data.research %}
      <section class="research-project" id="{{ item.id }}" aria-labelledby="{{ item.id }}-title">
        <div class="research-project-copy">
          <div>
            <p class="research-eyebrow"><span class="research-number">{% if forloop.index < 10 %}0{% endif %}{{ forloop.index }}</span> {{ item.method }}</p>
            <h2 id="{{ item.id }}-title">{{ item.title }}</h2>
          </div>
          <div class="research-project-summary">
            <p>{{ item.summary }}</p>
            <div class="research-links">
              <a href="{{ item.details | relative_url }}">Explore this project <span aria-hidden="true">&rarr;</span></a>
              {% if item.paper %}
                <a href="{{ item.paper }}">{{ item.paper_label }} <span aria-hidden="true">↗</span></a>
              {% endif %}
            </div>
          </div>
        </div>
        {% include research_media.liquid media=item %}
      </section>
    {% endfor %}
  </div>

  <p class="research-note">These projects include current work and earlier research by Kexin Zhang with collaborators. Explore each project for more figures, animations, and publications.</p>
</div>
