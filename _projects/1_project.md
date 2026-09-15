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

Page d'accueil

<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/cuisinemomo.png" title="Page d'accueil de Cuisine MOMO" class="img-fluid rounded z-depth-1" %} 
    </div> 
</div> 
<div class="caption"> 
    La page d'accueil (<code>index.html</code>) avec une section "hero" : un texte de bienvenue à gauche et une image de cuisine à droite. La mise en page est gérée avec Flexbox dans <code>accueil.css</code>, par-dessus les variables de couleurs définies dans <code>variables.css</code>. 
</div> 
<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/cuisinemomoaccueil2.png" title="Cartes de navigation sur la page d'accueil" class="img-fluid rounded z-depth-1" %} 
    </div> 
</div> 
<div class="caption"> 
    Toujours sur la page d'accueil, une deuxième section présente 3 cartes cliquables (Recettes, Techniques, Saisonnier), chacune menant vers sa propre page HTML. Construites avec Flexbox pour rester alignées et responsives sur mobile. 
</div>

Les autres pages du site

<div class="row"> 
    <div class="col-sm-6 mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/cuisinemomorecettes.png" title="Page des recettes" class="img-fluid rounded z-depth-1" %} 
    </div> 
    <div class="col-sm-6 mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/cuisinemomotechniques.png" title="Page des techniques de cuisine" class="img-fluid rounded z-depth-1" %} 
    </div> 
</div> 
<div class="row justify-content-sm-center"> 
    <div class="col-sm-6 mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/cuisinemomosaisonnier.png" title="Page des produits de saison" class="img-fluid rounded z-depth-1" %} 
    </div>
</div> 
<div class="caption"> 
    Dans l'ordre du menu : <b>Recettes</b> (<code>recettes.html</code>) liste les recettes sous forme de cartes avec portions, temps et difficulté ; <b>Techniques</b> (<code>techniques.html</code>) présente les bases en 3 colonnes (Coupes, Cuissons, Mesures & conversions) ; <b>Saisonnier</b> (<code>saisonnier.html</code>) affiche un tableau des produits disponibles par mois. Chaque page a son propre fichier CSS (<code>recettes.css</code>, <code>techniques.css</code>, <code>saisonnier.css</code>). 
</div>

Pied de page

<div class="row justify-content-sm-center"> 
    <div class="col-sm-8 mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/cuisinemomocontacts.png" title="Pied de page du site" class="img-fluid rounded z-depth-1" %} 
    </div> 
</div> 
<div class="caption"> 
    Le pied de page, présent sur toutes les pages, regroupe les coordonnées du cégep et des liens rapides vers les autres sections. Fait avec Flexbox dans <code>main.css</code>, le fichier de style commun à tout le site. 
</div>