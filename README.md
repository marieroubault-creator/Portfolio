# Portfolio · Marie Roubault

Page d'accueil qui référence mes réalisations en ligne, sous quatre onglets : sites en ligne, affiches (classées par lieu), supports de présentation et vidéos.

## Mettre en ligne sur GitHub Pages

1. Sur GitHub, créez un dépôt public nommé `marieroubault-creator.github.io` (le nom de votre compte suivi de `.github.io`).
2. Déposez-y `index.html` et ce `README.md` (bouton **Add file → Upload files**).
3. Allez dans **Settings → Pages**, choisissez **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
4. Au bout d'une minute, le portfolio est visible à l'adresse `https://marieroubault-creator.github.io/`.

## Organisation des dossiers du dépôt

```
index.html
README.md
cv.pdf
img/                  captures d'écran des 4 sites
affiches/
  saint-denis/        affiches de Saint-Denis
  saint-malo/         affiches de Saint-Malo
supports/             supports de présentation
videos/               vidéos (mp4)
```

Pour créer un dossier sur GitHub : **Add file → Upload files**, puis glissez vos fichiers déjà rangés dans des dossiers du même nom, ou **Add file → Create new file** et tapez `affiches/saint-denis/nom.pdf` dans le champ du nom.

## Ajouter vos affiches, supports et vidéos

Les onglets lisent des listes situées dans `index.html`, dans le bloc `VOS DOCUMENTS`, près de la fin du fichier (ouvrez-le dans GitHub avec l'icône crayon). Des lignes d'exemple sont déjà prévues, avec des titres à compléter : tant que les fichiers correspondants ne sont pas déposés, leurs liens mènent à une page d'erreur.

### Affiches

Deux listes : `AFFICHES_SAINT_DENIS` et `AFFICHES_SAINT_MALO`. Pour chaque affiche, adaptez une ligne :

```js
{ titre: "Affiche forum emploi", description: "Forum de septembre.", fichier: "affiches/saint-malo/forum-emploi.pdf" },
```

- `titre` : le nom affiché sous la vignette.
- `description` : une phrase courte (facultative).
- `fichier` : le chemin exact du fichier déposé, avec la même orthographe et la même extension.
- Pour ajouter un document, copiez une ligne complète ; pour en retirer un, supprimez sa ligne. Gardez la virgule en fin de ligne, sauf pour la dernière ligne de chaque liste.

Si le fichier est une image (`.png`, `.jpg`), elle sert directement d'aperçu. Pour un PDF, ajoutez si vous le souhaitez une capture de la première page :

```js
{ titre: "Affiche forum emploi", fichier: "affiches/saint-malo/forum-emploi.pdf", vignette: "affiches/saint-malo/forum-emploi-apercu.png" },
```

Le menu burger propose, sous « Affiches », deux raccourcis côte à côte : Saint-Denis et Saint-Malo.

### Supports de présentation

Liste `SUPPORTS`, avec le même fonctionnement, dans le dossier `supports/`.

### Vidéos

Liste `VIDEOS`. Deux possibilités :

```js
{ titre: "Présentation", description: "Ma vidéo.", fichier: "videos/presentation.mp4" },
{ titre: "Ma vidéo", description: "Sur YouTube.", youtube: "https://www.youtube.com/watch?v=XXXXXXXXXXX" },
```

- La vidéo s'ouvre dans une fenêtre de lecture au clic sur la vignette.
- Un fichier `.mp4` envoyé depuis le navigateur ne doit pas dépasser 25 Mo (100 Mo en ligne de commande). Pour une vidéo plus lourde, mettez-la sur YouTube (en « non répertoriée » si vous ne voulez pas qu'elle soit publique) et utilisez le champ `youtube`.
- Pour un fichier `.mp4`, la vignette montre une image de la vidéo si le navigateur le permet. Vous pouvez aussi indiquer `vignette: "videos/apercu.png"`.

## Faire apparaître les images de vos sites dans les vignettes

Tant qu'aucune capture n'est présente, chaque vignette de site affiche une illustration dessinée. Dès qu'un fichier du bon nom existe dans le dossier `img/`, la capture la remplace automatiquement.

| Projet | Fichier attendu |
|---|---|
| Parcours à la carte | `img/parcours-a-la-carte.png` |
| La Route du Rome | `img/route-du-rome.png` |
| Connect Emploi | `img/connect-emploi.png` |
| Atelier Senior | `img/atelier-senior.png` |

Faites une capture d'écran de chaque site (Windows : **Windows + Maj + S** ; Mac : **Cmd + Maj + 4**), enregistrez-la sous le nom indiqué et déposez-la dans le dossier `img`. Format conseillé : environ 1280 × 800 px, moins de 300 Ko.

## Personnaliser

- **E-mail** : dans `index.html`, remplacez `votre-adresse@exemple.fr` (deux occurrences).
- **CV** : déposez votre CV dans le dépôt sous le nom `cv.pdf`.
- **Textes** : relisez les descriptions des quatre sites, surtout celle d'Atelier Senior, et la section « À propos ».

## Typographie et palette

Police : Della Respira (Google Fonts), chargée automatiquement.

Douceurs : crème `#FFFBF6`, lavande `#E9E4FF`, menthe `#DFF3EA`, pêche `#FFE3D3`, ciel `#DDEBFF`.
Touches pop : corail `#FF5C7A`, soleil `#FFC93C`, violet `#7B5CFF`, turquoise `#19C3A6`.
