---
layout: page
title: Montréal Mic'd up
description: Mon site Web illustre plusieurs artistes de Montréal. Le but de celui-ci est de pouvoir mettre les artistes de Montréal de l’avant, car il y a beaucoup de talent dans la ville dans le domaine de la musique. Je trouve que ceux-ci méritent d’être connus et écoutés. Je vais partager des descriptions de ces artistes et quelques morceaux de leur discographie. Dans ce projet j'ai utilisé mes compétences dans le stack MERN (MongoDB, Express, React et Node.js).
img: assets/img/montrealmicdup.jpg
importance: 2
category: work
images:
    lightbox2: true

---
Liens: 

<a href="https://github.com/ShaniceDau/Montreal-Micdup.git" style="text-decoration: underline;">Voir le code sur GitHub</a>

<a href="https://foura5-projet-final-h26-shanicedaudier.onrender.com/" style="text-decoration: underline;">Voir le site Web</a>

Montréal Mic'd up est un site fait avec le stack MERN (MongoDB, Express, React et Node.js) qui met en valeur des artistes de la scène musicale montréalaise, avec une fiche descriptive et une chanson populaire pour chacun. Le site est disponible en français et en anglais. 

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
        <a href="{{ 'assets/img/mtlmicdup.png' | relative_url }}" data-lightbox="montreal-micdup" data-title="Page d'accueil - liste des artistes"><img src="{{ 'assets/img/mtlmicdup.png' | relative_url }}" alt="Page d'accueil - liste des artistes" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    La page d'accueil présente les artistes de Montréal sous forme de cartes (photo, catégorie, chanson populaire), avec une barre de recherche et un sélecteur de langue (FR/EN) en haut à droite. 
</div>

Fiche d'un artiste
<div class="row"> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mmdescription.png' | relative_url }}" data-lightbox="montreal-micdup" data-title="Description d'un artiste"><img src="{{ 'assets/img/mmdescription.png' | relative_url }}" alt="Description d'un artiste" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mmvideo.png' | relative_url }}" data-lightbox="montreal-micdup" data-title="Chanson populaire intégrée"><img src="{{ 'assets/img/mmvideo.png' | relative_url }}" alt="Chanson populaire intégrée" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    Chaque artiste a sa propre page : une bannière avec sa photo et son genre musical, une section "À propos" qui le présente, et plus bas la vidéo YouTube de sa chanson la plus populaire, intégrée directement dans la page. 
</div>

Inscription et connexion
<div class="row"> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mmregister.png' | relative_url }}" data-lightbox="montreal-micdup" data-title="Formulaire d'inscription"><img src="{{ 'assets/img/mmregister.png' | relative_url }}" alt="Formulaire d'inscription" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mmlogin.png' | relative_url }}" data-lightbox="montreal-micdup" data-title="Formulaire de connexion"><img src="{{ 'assets/img/mmlogin.png' | relative_url }}" alt="Formulaire de connexion" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    Le site permet de créer un compte (courriel, mot de passe, prénom, nom, acceptation des conditions) et de se connecter ensuite, avec l'authentification gérée côté serveur via Express et Node.js. 
</div>

Espace administration
<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mmconnecte.png' | relative_url }}" data-lightbox="montreal-micdup" data-title="Vue administrateur connecté"><img src="{{ 'assets/img/mmconnecte.png' | relative_url }}" alt="Vue administrateur connecté" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    Une fois connecté en tant qu'administrateur, un bandeau "Administration" apparaît en haut, avec les boutons "Ajouter un artiste", "Modifier" et "Supprimer" directement sur les cartes de la page d'accueil. 
</div> 
<div class="row"> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mmajout.png' | relative_url }}" data-lightbox="montreal-micdup" data-title="Formulaire d'ajout d'un artiste"><img src="{{ 'assets/img/mmajout.png' | relative_url }}" alt="Formulaire d'ajout d'un artiste" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/mmmodifier.png' | relative_url }}" data-lightbox="montreal-micdup" data-title="Formulaire de modification d'un artiste"><img src="{{ 'assets/img/mmmodifier.png' | relative_url }}" alt="Formulaire de modification d'un artiste" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    Le formulaire d'ajout d'un artiste (nom, catégorie, chanson populaire, image, description) et celui de modification, pré-rempli avec les données existantes (ici l'artiste Enima), pour corriger ou compléter une fiche déjà en ligne. 
</div>