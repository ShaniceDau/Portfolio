---
layout: page
title: Mémoire beauté
description: Memoire beauté est un site de jeu de mémoire. Il avait pour but de mettre de l'avant l'enregistrement de données dans le session storage et le local storage. 
img: assets/img/memoirebeaute.png
importance: 1
category: work
images:
    lightbox2: true

---
Lien: 

[Voir le code sur GitHub](https://github.com/ShaniceDau/memoirebeaute.git)

Mémoire beauté est un jeu de mémoire en JavaScript, où il fallait retrouver les paires de cartes (fruits, légumes et cosmétiques). Le nom du joueur est gardé dans le sessionStorage (le temps de la session), et les meilleurs scores sont sauvegardés dans le localStorage (persistant, même après avoir fermé le navigateur), avec un top 5 des meilleurs joueurs. 

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
        <a href="{{ 'assets/img/memoirebeaute.png' | relative_url }}" data-lightbox="memoire-beaute" data-title="Page d'accueil de Mémoire Beauté"><img src="{{ 'assets/img/memoirebeaute.png' | relative_url }}" alt="Page d'accueil de Mémoire Beauté" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    La page d'accueil (<code>index.html</code>) où le joueur entre son nom (enregistré dans le <code>sessionStorage</code>) avant de commencer, et où s'affiche déjà le Top 5 des meilleurs scores, chargé depuis le <code>localStorage</code>. 
</div>

Règles du jeu

<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mbregles.png' | relative_url }}" data-lightbox="memoire-beaute" data-title="Page des règles du jeu"><img src="{{ 'assets/img/mbregles.png' | relative_url }}" alt="Page des règles du jeu" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    La page <code>regles.html</code> explique le but du jeu et les objectifs avant que le joueur clique sur "Prêt" pour lancer la partie. 
</div>

Le jeu

<div class="row"> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mbjeu.png' | relative_url }}" data-lightbox="memoire-beaute" data-title="Grille de jeu en cours"><img src="{{ 'assets/img/mbjeu.png' | relative_url }}" alt="Grille de jeu en cours" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mbjeu2.png' | relative_url }}" data-lightbox="memoire-beaute" data-title="Grille de jeu et Top 5"><img src="{{ 'assets/img/mbjeu2.png' | relative_url }}" alt="Grille de jeu et Top 5" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    La page <code>jeu.html</code> affiche la grille de cartes à retourner, avec un chronomètre et un compteur de coups en haut. Une fois la partie terminée, le score est comparé au Top 5 sauvegardé dans le <code>localStorage</code> et mis à jour si besoin. 
</div>