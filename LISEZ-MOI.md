# Site Brad Bitt — version 1.4

## Ce qui change

* **Le jeu n'est plus « suspendu ».** Partout où le site parlait d'une suspension
  pour une durée indéterminée, il annonce maintenant une **sortie visée courant 2027** :
  bannière d'accueil, lettre de Brad Bitt, carte du jeu, nouveautés.
* **Refonte visuelle complète** de la page d'accueil (typographie, thèmes clair et
  sombre, en-tête en verre, hero animé, cartes d'épisodes avec vignettes YouTube).
* **Le lien Canva a disparu.** Le bouton « Découvrir » ouvre désormais `jeu.html`,
  une page de présentation qui se découvre en faisant défiler : chaque section
  apparaît à mesure qu'on descend, et la capture du niveau se transforme
  d'extérieur en intérieur au fil du défilement.

## Ce qu'il faut mettre en ligne

Copie ces fichiers **à la racine du site**, à côté de ton `index.html` actuel :

```
index.html          (remplace l'ancien)
style.css           (remplace l'ancien)
script.js           (remplace l'ancien)
jeu.html            (nouveau)
jeu.css             (nouveau)
jeu.js              (nouveau)
images/jeu/…        (nouveau dossier — à AJOUTER dans images/, sans rien effacer)
```

**Important :** le dossier `images/` livré ici ne contient que le sous-dossier `jeu/`.
Il faut le **fusionner** avec ton dossier `images/` existant, pas le remplacer :
tes logos (`logo bb site clair.png`, `logo bb site sombre.png`) et le dossier
`images/web/` (favicons, `site.webmanifest`) restent indispensables.

Aucune dépendance, aucun script de build. Les polices viennent de Google Fonts.

## Contenu de images/jeu/

| Fichier | D'où il vient |
|---|---|
| `brad-planche.png` | la planche de sprites de Brad du prototype, agrandie ×4 |
| `ennemis/*.png` | les sprites des Serra du prototype, agrandis ×6 |
| `uniformes/*.png` | tes onze uniformes, détourés du fond blanc et remis à l'échelle |
| `captures/*.png` | trois captures prises directement dans le prototype en ligne |
| `skyline-*.svg` | silhouettes de tours générées, utilisées comme masques CSS |
| `logo-imagine.png`, `logo-hwr.png` | les logos des studios du prototype |

## Deux ou trois choses à vérifier de ton côté

* **Quatorze pistes.** La page annonce « quatorze pistes déjà composées » :
  c'est le nombre de fichiers dans ton dossier `mais les musiques`. À ajuster si
  tu comptes autrement.
* **BRADDY3000.** Tes notes le présentent à la fois comme l'adversaire que Brad
  pourchasse et comme l'assistant de la boutique. La page a retenu la seconde
  version (narrateur et assistant) et laisse Kirby67 dans le rôle de la cible.
* **Serra-Boost.** Les notes le décrivaient comme invulnérable et lanceur de bombes ;
  dans le prototype c'est le coureur. La page décrit le coureur et mentionne la
  variante invulnérable comme prévue.
* **Les captures** viennent du prototype 05 tel qu'il est en ligne aujourd'hui.
  Il faudra les refaire quand le jeu aura avancé.

## Réglages utiles

* `script.js` → `NEWS_VERSION` : incrémente à chaque mise à jour pour réafficher
  la pastille « nouveautés », et ajoute une entrée en haut de `NEWS_HISTORY`.
* `script.js` → `PANELS.letter` : le texte de la lettre.
* `jeu.js` → le fondu entre les deux zones se règle dans `majZone()`.
