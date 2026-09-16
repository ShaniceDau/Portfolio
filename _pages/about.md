---
layout: about
title: Portfolio
permalink: /
subtitle: Bienvenue dans mon portfolio.

profile:
  align: right
  image: femmeinfo.png
  image_circular: false # crops the image to make it circular
  more_info:

---

Mon nom est Shanice Daudier une passionnée du developpement' d'application. Ce site web contient un amas de projet que j'ai réalisé durant mon parcours dans ce domaine.

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