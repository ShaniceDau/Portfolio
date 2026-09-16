---
layout: about
title: Portfolio
permalink: /
subtitle: Bienvenue dans mon portfolio.

profile:
  align: right
  image: femmeinfo.jpg
  image_circular: false # crops the image to make it circular
  more_info:

---

<style> 
  .profile { 
    max-width: 200px; 
  } 
  .profile img { 
    border: 5px solid transparent; 
    background: linear-gradient(#fff, #fff) padding-box, linear-gradient(135deg, #ec4899, #a855f7, #6366f1) border-box; 
    box-shadow: 0 8px 30px rgba(0, 0, 0, 0.2); 
    transition: transform 0.35s ease, box-shadow 0.35s ease; 
  } 
  .profile img:hover { 
    transform: scale(1.04) rotate(1deg); box-shadow: 0 12px 40px rgba(0, 0, 0, 0.3); 
  } 
</style>

Mon nom est Shanice Daudier, une passionnée du développement d'application. Ce site web contient un amas de projet que j'ai réalisé durant mon parcours dans ce domaine.

<div style="margin-top: 5rem; padding-top: 2.5rem; border-top: 1px solid var(--global-divider-color, #e0e0e0);">


Projets

<!-- Grille de projets, identique à _pages/projects.md --> 

<div class="projects"> 
{% if site.enable_project_categories and page.display_categories %} 
  <!-- Display categorized projects --> 
  {% for category in page.display_categories %} 
  <a id="{{ category }}" href=".#{{ category }}"> 
    <h2 class="category">{{ category }}</h2> 
  </a> 
  {% assign categorized_projects = site.projects | where: "category", category %} 
  {% assign sorted_projects = 
  categorized_projects | sort: "importance" %} 
  <!-- Generate cards for each project --> 
  {% if page.horizontal %} 
  <div class="container"> 
    <div class="row row-cols-1 row-cols-md-2"> 
    {% for project in sorted_projects %} 
      {% include projects_horizontal.liquid %} 
    {% endfor %} 
    </div>
  </div> {% else %} 
  <div class="row row-cols-1 row-cols-md-3"> 
    {% for project in sorted_projects %} 
      {% include projects.liquid %} 
    {% endfor %} 
  </div> 
  {% endif %} 
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

<!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container"> 
    <div class="row row-cols-1 row-cols-md-2"> 
    {% for project in sorted_projects %} 
      {% include projects_horizontal.liquid %} 
    {% endfor %} 
    </div> 
  </div> 
    {% else %} 
    <div class="row row-cols-1 row-cols-md-3"> 
      {% for project in sorted_projects %} 
        {% include projects.liquid %} 
      {% endfor %} 
      </div> 
      {% endif %}
    {% endif %} 
    </div> 
</div>