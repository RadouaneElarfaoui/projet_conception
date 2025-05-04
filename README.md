# Rapport de Projet de Conception CATIA V5

Ce dépôt contient tous les fichiers nécessaires pour rédiger un rapport complet sur votre projet de conception réalisé avec CATIA V5.

## Structure des fichiers

- `rapport_projet_conception.tex` : Fichier principal du rapport LaTeX
- `modele_documentation_piece.tex` : Modèle pour documenter chaque pièce
- `modele_documentation_assemblage.tex` : Modèle pour documenter l'assemblage
- `modele_documentation_dessins.tex` : Modèle pour documenter les dessins techniques
- `operations_catia_v5.md` : Liste des opérations CATIA V5 à documenter
- `guide_redaction.md` : Guide pour vous aider à remplir le rapport
- `images/` : Dossier pour stocker les captures d'écran de CATIA V5

## Comment utiliser ces fichiers

### 1. Préparation des images

1. Faites des captures d'écran de vos modèles, assemblages et dessins dans CATIA V5
2. Enregistrez-les dans le dossier `images/` au format PNG
3. Utilisez des noms explicites (ex: `piece1_3d.png`, `assemblage_complet.png`)

### 2. Personnalisation du rapport

1. Ouvrez le fichier `rapport_projet_conception.tex`
2. Remplacez les informations générales (nom, titre du projet)
3. Complétez chaque section en utilisant les modèles fournis

### 3. Documentation des pièces

Pour chaque pièce importante de votre projet:

1. Consultez le fichier `modele_documentation_piece.tex`
2. Copiez son contenu dans la section correspondante de votre rapport
3. Remplacez les placeholders [texte entre crochets] par vos informations
4. Référencez les images que vous avez préparées

### 4. Documentation de l'assemblage

1. Consultez le fichier `modele_documentation_assemblage.tex`
2. Copiez son contenu dans la section correspondante de votre rapport
3. Adaptez la structure à votre propre assemblage
4. Détaillez les contraintes utilisées

### 5. Documentation des dessins techniques

1. Consultez le fichier `modele_documentation_dessins.tex`
2. Copiez son contenu dans les sections correspondantes
3. Décrivez vos choix de représentation, cotation, etc.

## Compilation du rapport

Pour générer le PDF final:

1. Assurez-vous d'avoir une distribution LaTeX installée (TeX Live, MiKTeX)
2. Compilez le fichier principal avec la commande:
   ```
   pdflatex rapport_projet_conception.tex
   ```
3. Pour générer correctement la table des matières, compilez deux fois:
   ```
   pdflatex rapport_projet_conception.tex
   pdflatex rapport_projet_conception.tex
   ```

## Conseils supplémentaires

- Consultez `operations_catia_v5.md` pour vous assurer de bien documenter les fonctionnalités CATIA que vous avez utilisées
- Suivez les instructions du `guide_redaction.md` pour un rapport complet et bien structuré
- N'oubliez pas de décommenter les lignes `\includegraphics` dans le rapport quand vous ajoutez vos images

## Exemple de section complétée

Pour vous aider à comprendre comment utiliser les modèles, voici un exemple de section complétée:

```latex
\subsection{Modélisation du Support principal}

\subsubsection{Description et fonction}
Cette pièce a pour fonction principale de supporter l'axe de rotation principal. Elle est caractérisée par sa forme en U avec deux alésages alignés de diamètre 15mm.

\subsubsection{Étapes de modélisation}
Pour réaliser cette pièce, nous avons procédé comme suit:

\begin{enumerate}
    \item \textbf{Création de l'esquisse principale} : 
    \begin{itemize}
        \item Plan de travail : Plan XY
        \item Éléments dessinés : Rectangle de 80x50mm avec ligne de symétrie verticale
        \item Contraintes appliquées : Symétrie par rapport à l'axe Y, horizontalité et verticalité des côtés
        \item Cotation : 80mm de largeur, 50mm de hauteur
    \end{itemize}
    
    \item \textbf{Opération volumique principale} : 
    \begin{itemize}
        \item Fonction utilisée : Extrusion (Pad)
        \item Paramètres : Extrusion de 20mm dans la direction Z positif
    \end{itemize}
    
    ...
\end{enumerate}
``` 