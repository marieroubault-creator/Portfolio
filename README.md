# Portfolio · Marie Roubault

Page d'accueil qui référence mes réalisations en ligne : sites, affiches et supports de présentation, présentés sous trois onglets.

## Mettre en ligne sur GitHub Pages

1. Sur GitHub, créez un dépôt public nommé `marieroubault-creator.github.io` (le nom de votre compte suivi de `.github.io`).
2. Déposez-y `index.html` et ce `README.md` (bouton **Add file → Upload files**).
3. Allez dans **Settings → Pages**, choisissez **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
4. Au bout d'une minute, le portfolio est visible à l'adresse `https://marieroubault-creator.github.io/`.

## Ajouter vos affiches et supports de présentation

Les onglets **Affiches** et **Supports de présentation** lisent une liste située dans `index.html`. Trois affiches et deux supports sont déjà prévus, avec des titres à compléter.

1. Dans votre dépôt, créez les dossiers `affiches` et `supports` (**Add file → Upload files**, puis glissez vos fichiers dans un dossier du même nom).
2. Déposez vos fichiers (PDF recommandé, ou image `.png` / `.jpg`).
3. Ouvrez `index.html` dans GitHub (icône crayon) et cherchez le bloc `VOS DOCUMENTS`, près de la fin du fichier.
4. Pour chaque document, adaptez une ligne :

```js
{ titre: "Affiche forum emploi", description: "Affiche du forum de septembre.", fichier: "affiches/forum-emploi.pdf" },
```

- `titre` : le nom affiché sous la vignette.
- `description` : une phrase courte (facultative, vous pouvez la supprimer).
- `fichier` : le chemin exact du fichier déposé, avec la même orthographe et la même extension.
- Pour ajouter un document, copiez une ligne complète ; pour en retirer un, supprimez sa ligne. Gardez la virgule en fin de ligne, sauf pour la dernière ligne de la liste.

**Aperçu de la vignette** :
- Si le fichier est une image (`.png`, `.jpg`), elle sert directement d'aperçu.
- Si c'est un PDF, la vignette est une illustration. Pour afficher un vrai aperçu, ajoutez une capture de la première page et indiquez-la ainsi :

```js
{ titre: "Affiche forum emploi", fichier: "affiches/forum-emploi.pdf", vignette: "affiches/forum-emploi-apercu.png" },
```

Les compteurs des onglets se mettent à jour tout seuls.

## Faire apparaître les images de vos sites dans les vignettes

Tant qu'aucune capture n'est présente, chaque vignette de site affiche une illustration dessinée. Dès qu'un fichier du bon nom existe dans le dossier `img/`, la capture la remplace automatiquement.

| Projet | Fichier attendu |
|---|---|
| Parcours à la carte | `img/parcours-a-la-carte.png` |
| La Route du Rome | `img/route-du-rome.png` |
| Connect Emploi | `img/connect-emploi.png` |
| Atelier Senior | `img/atelier-senior.png` |

Faites une capture d'écran de chaque site (Windows : **Windows + Maj + S** ; Mac : **Cmd + Maj + 4**), enregistrez-la sous le nom indiqué et déposez-la dans le dossier `img` du dépôt. Format conseillé : environ 1280 × 800 px, moins de 300 Ko.

## Personnaliser

- **E-mail** : dans `index.html`, remplacez `votre-adresse@exemple.fr` (deux occurrences).
- **CV** : déposez votre CV dans le dépôt sous le nom `cv.pdf`.
- **Textes** : relisez les descriptions des quatre sites, surtout celle d'Atelier Senior, et la section « À propos ».

## Typographie et palette

Police : Della Respira (Google Fonts), chargée automatiquement.

Douceurs : crème `#FFFBF6`, lavande `#E9E4FF`, menthe `#DFF3EA`, pêche `#FFE3D3`, ciel `#DDEBFF`.
Touches pop : corail `#FF5C7A`, soleil `#FFC93C`, violet `#7B5CFF`, turquoise `#19C3A6`.
