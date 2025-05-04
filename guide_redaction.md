# Guide pour la rédaction du rapport de projet CATIA V5

Ce document vous aidera à compléter votre rapport LaTeX sur votre projet de conception réalisé avec CATIA V5.

## Structure du rapport

Le rapport est organisé en chapitres:
1. Introduction
2. Conception des pièces
3. Assemblage
4. Dessins de définition
5. Dessin d'ensemble
6. Analyse critique et conclusion

## Conseils pour remplir le rapport

### Informations générales
- Remplacez "Votre Nom" par votre nom réel dans l'entête du document
- Ajoutez une description précise de votre projet dans l'introduction

### Images à ajouter
Pour chaque section où une figure est mentionnée:
1. Faites une capture d'écran de CATIA V5 montrant l'élément concerné
2. Enregistrez l'image au format PNG dans le dossier "images"
3. Décommentez la ligne `\includegraphics` dans le fichier .tex
4. Remplacez "nom_image.png" par le nom réel de votre fichier

### Conception des pièces
Pour chaque pièce importante:
1. Ajoutez son nom dans la liste des pièces
2. Décrivez précisément les étapes de modélisation:
   - Quelles esquisses avez-vous réalisées?
   - Quelles fonctions avez-vous utilisées (extrusion, révolution, balayage...)?
   - Quels paramètres avez-vous définis?
   - Quelles autres opérations avez-vous effectuées (congés, chanfreins...)?

### Assemblage
1. Décrivez la structure hiérarchique de votre assemblage
2. Détaillez les contraintes utilisées pour positionner les pièces:
   - Contraintes de coïncidence
   - Contraintes de distance
   - Contraintes d'angle
   - Autres contraintes spécifiques

### Dessins de définition
1. Décrivez les normes de cotation que vous avez suivies
2. Précisez comment vous avez déterminé:
   - Les tolérances dimensionnelles
   - Les tolérances géométriques
   - Les états de surface

### Dessin d'ensemble
1. Complétez la nomenclature avec les informations de toutes vos pièces
2. Décrivez comment vous avez organisé les vues et coupes

### Analyse critique et conclusion
1. Notez les difficultés techniques que vous avez rencontrées
2. Expliquez comment vous les avez surmontées
3. Réfléchissez aux compétences que vous avez développées

## Commandes LaTeX utiles

- Pour ajouter une nouvelle pièce à la liste: `\item Pièce X: [Nom de la pièce]`
- Pour ajouter une image: `\includegraphics[width=0.7\textwidth]{images/nom_image.png}`
- Pour créer une nouvelle section: `\section{Titre de la section}`
- Pour créer une sous-section: `\subsection{Titre de la sous-section}`
- Pour ajouter une référence à une figure: `\ref{fig:nom_label}`

## Compilation du document LaTeX

Pour compiler votre document LaTeX:
1. Installez une distribution LaTeX comme TeX Live ou MiKTeX
2. Compilez avec la commande: `pdflatex rapport_projet_conception.tex`
3. Compilez deux fois pour générer correctement la table des matières 