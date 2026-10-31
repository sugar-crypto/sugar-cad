# Sugar CAD · CAO par le code

Atelier de CAO 3D dans le navigateur : on décrit ou on code une pièce, on la règle, on la vérifie, on la met en plan et on l'exporte. Aucun serveur, aucune installation : un seul fichier `index.html`.

**Démo en ligne :** https://sugar-crypto.github.io/sugar-cad/

## Fonctionnalités

- **Modélisation par le code** (JavaScript, moteur JSCAD) avec aperçu 3D en direct
- **Assistant de génération** : « plaque 100×60×10 avec 4 trous » (FR, EN, العربية)
- **Paramétrique** : les constantes marquées `// @p Nom` deviennent des curseurs
- **Bibliothèque de pièces** et exemples prêts à modifier
- **Dessin technique** : 3 vues cotées, arêtes cachées, cartouche
- **Analyse** : masse selon le matériau, nomenclature (BOM), vérification de la pièce
- **Assemblages**, mesure, coupe, couleurs par corps, versions avec aperçu
- **Calculs d'ingénieur** (indicatifs, à vérifier avec une référence reconnue)
- **Import** : STL, DXF, image → programme
- **Export** : STL, OBJ, 3MF, DXF, SVG, PDF, script Python (CadQuery)
- Interface **français / English / العربية**, mode clair et sombre

## Utilisation

1. Ouvre le lien de la démo, ou télécharge `index.html` et ouvre-le dans un navigateur récent.
2. Écris du code, termine par `return` suivi de la pièce. Unité : mm, axe Z vers le haut.
3. Exemple minimal :

```js
const L = 100 // @p Longueur
const W = 60  // @p Largeur
const H = 10  // @p Épaisseur
return cuboid({size: [L, W, H]})
```

## Notes

- Une connexion internet est nécessaire au premier chargement (bibliothèques JSCAD, three.js, jsPDF via CDN).
- Les projets sont enregistrés localement dans le navigateur de chaque utilisateur.
- N'importe que des projets `.json` de confiance : ils contiennent du code exécuté dans la page.
- Projet indépendant, non affilié à Dassault Systèmes ; SolidWorks est une marque de ses propriétaires. Les résultats de calcul sont indicatifs.

## Licence

[MIT](LICENSE)
