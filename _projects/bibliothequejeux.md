---
layout: page
title: Bibliothèque de jeux
description: Le site de Bibliothèque de jeux a été fait avec REACT. C'est mon premier projet avec ce framework. Il y a les fonctionnalités d'ajouter un jeu, de modifier un jeu et de le supprimer, mais uniquement lorsqu'on est connecté. Sinon, ces fonctionnalités ne sont pas accessibles.
img: assets/img/bibliothequejeux.png
importance: 2
category: work

---

Lien:

<a href="https://github.com/ShaniceDau/Bibliotheque-De-Jeux.git" style="text-decoration: underline;">Voir le code sur GitHub</a>

Bibliothèque de jeux est mon premier projet fait avec React. L'état de connexion est géré via le Context API (AuthContext.js), ce qui permet d'afficher ou de cacher les boutons "Ajouter un jeu", "Modifier" et "Supprimer" selon que l'utilisateur est connecté ou non. 

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


Liste des jeux (visiteur non connecté)
<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/bibliothequejeux.png' | relative_url }}" data-lightbox="bibliotheque-jeux" data-title="Liste des jeux"><img src="{{ 'assets/img/bibliothequejeux.png' | relative_url }}" alt="Liste des jeux" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    La page d'accueil liste les jeux avec une barre de recherche. Sans être connecté, seuls les boutons "Jeux", "Connexion" et "S'inscrire" sont visibles dans le menu — pas de bouton "Ajouter un jeu" ni de boutons "Modifier"/"Supprimer" sur les cartes. 
</div>

Connexion
<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/connexion.png' | relative_url }}" data-lightbox="bibliotheque-jeux" data-title="Formulaire de connexion"><img src="{{ 'assets/img/connexion.png' | relative_url }}" alt="Formulaire de connexion" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    Le formulaire de connexion (composant <code>LoginForm.jsx</code>). Une fois connecté, le <code>AuthContext</code> met à jour l'état de l'application et débloque les fonctionnalités de gestion des jeux. 
</div>

Une fois connecté
<div class="row justify-content-sm-center"> 
    <div class="col-sm-12 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/connecte.png' | relative_url }}" data-lightbox="bibliotheque-jeux" data-title="Liste des jeux, utilisateur connecté"><img src="{{ 'assets/img/connecte.png' | relative_url }}" alt="Liste des jeux, utilisateur connecté" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    Connecté, le bouton "Ajouter un jeu" apparaît dans le menu et sur la page, et chaque carte affiche maintenant les boutons "Modifier" et "Supprimer". 
</div>

Ajout d'un jeu
<div class="row"> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/ajout.png' | relative_url }}" data-lightbox="bibliotheque-jeux" data-title="Formulaire d'ajout d'un jeu"><img src="{{ 'assets/img/ajout.png' | relative_url }}" alt="Formulaire d'ajout d'un jeu" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
    <div class="col-sm-6 mt-3 mt-md-0"> 
        <a href="{{ 'assets/img/suppression.png' | relative_url }}" data-lightbox="bibliotheque-jeux" data-title="Confirmation de suppression"><img src="{{ 'assets/img/suppression.png' | relative_url }}" alt="Confirmation de suppression" class="img-fluid rounded z-depth-1">
        </a> 
    </div> 
</div> 
<div class="caption"> 
    Le formulaire (<code>GameForm.jsx</code>) pour ajouter un nouveau jeu (titre, catégorie, nombre de joueurs, durée), et une fenêtre modale (<code>modal.jsx</code>) qui demande une confirmation avant de supprimer un jeu, pour éviter les suppressions accidentelles. 
</div>