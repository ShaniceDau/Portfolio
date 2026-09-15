---
layout: page
title: Cuisine Momo
description: Cuisne Momo est un projet de découverte de cuisine pour le cégep Montmorency. Ce projet a été fait uniquement avec du HTML et du CSS.
img: assets/img/cuisinemomo.png
importance: 1
category: work
---
Lien: 

[Voir le code sur GitHub](https://github.com/ShaniceDau/Cuisine-Momo.git)

Cuisine MOMO est un site multi-pages fait entièrement en HTML et CSS (sans framework). Le style commun (couleurs, polices) est centralisé dans un fichier variables.css, et chaque page a ensuite son propre fichier CSS dédié (accueil, recettes, techniques, saisonnier).
    ---

<style> 
    .al-lightbox-overlay { 
        background: rgba(0, 0, 0, 0.6) !important; 
    }
    .al-lightbox-figure { 
        max-width: min(65vw, 800px) !important; 
        max-height: 70vh !important; 
    } 
    .al-lightbox-image { 
        max-height: calc(70vh - 3rem) !important; 
        box-shadow: 0 10px 40px rgba(0, 0, 0, 0.5); 
        border-radius: 8px; 
    }
    .al-lightbox-close { 
        top: 1rem !important; 
        right: 1rem !important; 
        left: auto !important; 
        font-size: 1rem !important; 
        font-family: inherit; 
        background: rgba(0, 0, 0, 0.6) !important; 
        padding: 0.4rem 0.9rem !important; 
        border-radius: 6px !important; 
        display: inline-flex; 
        align-items: center; 
        gap: 0.4rem; 
    } 
</style> 

<script> window.addEventListener("load", function () { var closeBtn = document.querySelector(".al-lightbox-close"); if (closeBtn) { closeBtn.innerHTML = "&larr; Retour"; closeBtn.setAttribute("aria-label", "Retour à la page du projet"); } }); 
</script>

Page d'accueil

<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/cuisinemomo.png' | relative_url }}" data-lightbox="cuisine-momo" data-title="Page d'accueil de Cuisine MOMO">
        <img src="{{ 'assets/img/cuisinemomo.png' | relative_url }}" alt="Page d'accueil de Cuisine MOMO" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    La page d'accueil (<code>index.html</code>) avec une section "hero" : un texte de bienvenue à gauche et une image de cuisine à droite. La mise en page est gérée avec Flexbox dans <code>accueil.css</code>, par-dessus les variables de couleurs définies dans <code>variables.css</code>. 
</div> 
<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/cuisinemomoaccueil2.png' | relative_url }}" data-lightbox="cuisine-momo" data-title="Cartes de navigation sur la page d'accueil">
        <img src="{{ 'assets/img/cuisinemomoaccueil2.png' | relative_url }}" alt="Cartes de navigation sur la page d'accueil" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    Toujours sur la page d'accueil, une deuxième section présente 3 cartes cliquables (Recettes, Techniques, Saisonnier), chacune menant vers sa propre page HTML. Construites avec Flexbox pour rester alignées et responsives sur mobile. 
</div>

Les autres pages du site

<div class="row"> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/cuisinemomorecettes.png' | relative_url }}" data-lightbox="cuisine-momo" data-title="Page des recettes">
        <img src="{{ 'assets/img/cuisinemomorecettes.png' | relative_url }}" alt="Page des recettes" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/cuisinemomotechniques.png' | relative_url }}" data-lightbox="cuisine-momo" data-title="Page des techniques de cuisine"><img src="{{ 'assets/img/cuisinemomotechniques.png' | relative_url }}" alt="Page des techniques de cuisine" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="row justify-content-sm-center"> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/cuisinemomosaisonnier.png' | relative_url }}" data-lightbox="cuisine-momo" data-title="Page des produits de saison"><img src="{{ 'assets/img/cuisinemomosaisonnier.png' | relative_url }}" alt="Page des produits de saison" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    Dans l'ordre du menu : <b>Recettes</b> (<code>recettes.html</code>) liste les recettes sous forme de cartes avec portions, temps et difficulté ; <b>Techniques</b> (<code>techniques.html</code>) présente les bases en 3 colonnes (Coupes, Cuissons, Mesures & conversions) ; <b>Saisonnier</b> (<code>saisonnier.html</code>) affiche un tableau des produits disponibles par mois. Chaque page a son propre fichier CSS (<code>recettes.css</code>, <code>techniques.css</code>, <code>saisonnier.css</code>). 
</div>

Pied de page

<div class="row justify-content-sm-center"> 
    <div class="col-sm-8 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/cuisinemomocontacts.png' | relative_url }}" data-lightbox="cuisine-momo" data-title="Pied de page du site"><img src="{{ 'assets/img/cuisinemomocontacts.png' | relative_url }}" alt="Pied de page du site" class="img-fluid rounded z-depth-1">
        </a>
    </div> 
</div> 
<div class="caption"> 
    Le pied de page, présent sur toutes les pages, regroupe les coordonnées du cégep et des liens rapides vers les autres sections. Fait avec Flexbox dans <code>main.css</code>, le fichier de style commun à tout le site. 
</div>