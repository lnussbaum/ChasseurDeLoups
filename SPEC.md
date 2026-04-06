# Spécifications du Jeu : Chasseur de Loups

## 1. Concept du Jeu
"Chasseur de Loups" est une variante du célèbre jeu Démineur adaptée pour les enfants. L'objectif est de découvrir toutes les cases de la forêt sans tomber sur un loup caché.

## 2. Contraintes Techniques
- **Format** : Application web dans un **fichier HTML unique** (`index.html`).
- **Langages** : HTML5, CSS3 (Vanilla) et JavaScript (Vanilla).
- **Rendu** : Entièrement "responsive", optimisé pour les écrans de téléphones portables.
- **Assets** : Les icônes et illustrations (loups, drapeaux, etc.) doivent être intégrées via SVG ou CSS pour conserver le format fichier unique.

## 3. Mécaniques de Jeu
- **La Grille** : Un champ de cases carrées. Certaines cachent des loups.
- **Les Indices** : Cliquer sur une case révèle soit un loup (défaite), soit un chiffre indiquant combien de loups se trouvent dans les 8 cases adjacentes.
- **Les Niveaux** :
    - **Apprenti** : 6x6 cases, 5 loups (Le plus petit).
    - **Explorateur** : 8x8 cases, 8 loups.
    - **Chasseur** : 9x9 cases, 10 loups (Standard Débutant).
    - **Grand Chasseur** : 12x12 cases, 20 loups.
- **Modes d'action** : Un bouton sélecteur en bas de l'écran permet de basculer entre :
    - **Mode Découverte** (Icône Traces de pas) : Suit la piste de l'enfant qui marche et révèle le contenu de la case.
    - **Mode Couteau** (Icône Couteau) : Plante un couteau pour marquer l'emplacement supposé d'un loup.

## 4. Interface Utilisateur (UI)
- **Thème Visuel** : Forêt mystérieuse mais colorée, adaptée aux enfants.
- **Grille de jeu** : Centrée, avec des cases assez grandes pour être cliquées facilement au doigt.
- **Barre d'outils (Bas)** :
    - Un interrupteur visuel clair (Toggle) pour changer de mode.
    - Compteur de loups restants (drapeaux posés).
    - Chronomètre simple.
- **Menu de démarrage** : Choix de la difficulté.

## 5. États du Jeu
- **Victoire** : Écran joyeux avec un message de félicitations et un bouton pour rejouer.
- **Défaite (Game Over)** :
    - Affichage d'une illustration **un peu terrifiante** du "Grand Méchant Loup" (style conte de fées, yeux jaunes, grandes dents).
    - Vibrations légères (si supporté par le navigateur) pour l'effet de surprise.
    - Révélation de tous les loups restants sur la grille.

## 6. Accessibilité & Ergonomie
- Pas de clic droit nécessaire (le mode drapeau gère cela via le sélecteur).
- Couleurs contrastées.
- Feedback visuel immédiat lors d'un clic sur une case.
