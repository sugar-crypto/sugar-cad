# sugar · CAO par le code

Atelier de CAO 3D dans le navigateur : on décrit ou on code une pièce, on la règle, on la vérifie, on la met en plan, on l'exporte.

## Fonctions
- Page d'accueil, thème gris sombre/clair, **couleur d'accent au choix** (pastilles + sélecteur), FR · EN · العربية
- **Assistant** (règles, hors ligne) : « plaque 100×60×10 avec 4 trous » → code paramétrique
- **Paramètres** : curseurs `// @p` qui modifient la pièce en direct
- **Pièces** : bibliothèque (mécanique, électronique, architecture, drone)
- **Dessin technique** : 3 vues cotées, arêtes cachées, cartouche, export SVG/PDF
- **Analyse** : matériau et masse, vérification de conception, nomenclature CSV, versions avec aperçu
- Export : STL, OBJ, 3MF, STEP (facettes), SVG, DXF, PDF
- Onglet Python : script CadQuery pour un vrai STEP B-rep (`pip install cadquery`)

## Limites
Le moteur est un moteur de maillages : le STEP du site est en facettes. Un STEP B-rep éditable vient du script CadQuery. La vérification et le dessin sont approximatifs.

## Publier (GitHub Pages)
Settings → Pages → Branch `main` / root.
