---
layout: page
title: Jeu Boggle
description: Le but de ce projet était de développer une application graphique client/serveur. À partir d’un projet vide, il fallait construire une application étape par étape. L’application contient trois pages, dont une où il y a un jeu 2d implanté.
img: assets/img/jeuboggle.jpg
redirect: 
importance: 3
category: work
images:
    lightbox2: true

---
<div style="display: inline-flex; align-items: center; gap: 0.5rem; background: linear-gradient(135deg, #f5c518, #f7a600); color: #1a1a1a; font-weight: 600; padding: 0.5rem 1rem; border-radius: 999px; margin-bottom: 1rem;"> ⭐ Projet vedette du cours Environnement graphique - Collège Montmorency </div>

Jeu Boggle est une application graphique client/serveur en Java (JavaFX), construite étape par étape à partir d'un projet vide. Le but est de former des mots en cliquant sur des lettres adjacentes sur la grille avant la fin du temps imparti ; les meilleurs joueurs et leurs scores s'affichent en temps réel dans le panneau de droite. 

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

Aperçu du jeu
<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/jeuboggle.png' | relative_url }}" data-lightbox="jeu-boggle" data-title="Grille du jeu Boggle"><img src="{{ 'assets/img/jeuboggle.png' | relative_url }}" alt="Grille du jeu Boggle" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    La grille de jeu avec les lettres à sélectionner et, à droite, le classement en direct des joueurs avec leur lettre courante et leur temps. 
</div>

Vidéo de démonstration
<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> 
        <video controls preload="metadata" poster="{{ 'assets/img/jeuboggle.png' | relative_url }}" class="img-fluid rounded z-depth-1" style="width: 100%;"><source src="{{ 'assets/img/shanicejeuboggle.webm' | relative_url }}" type="video/webm">Ton navigateur ne supporte pas la lecture de cette vidéo.</video>
    </div> 
</div> 
<div class="caption"> 
    Une courte démonstration du jeu en action, montrant la sélection des lettres et le classement des joueurs se mettre à jour en temps réel. 
</div>