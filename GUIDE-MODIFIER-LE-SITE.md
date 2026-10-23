# Modifier, corriger ou ajouter du texte sur votre site

Une fois le site en ligne sur GitHub, vous modifiez tout **directement dans votre navigateur**, sans rien installer.
Chaque modification enregistrée met le site à jour automatiquement en 2 à 5 minutes.

## La méthode (valable pour tous les fichiers)

1. Allez sur `https://github.com/VOTRE-IDENTIFIANT/VOTRE-IDENTIFIANT.github.io` et connectez-vous.
2. Cliquez sur les dossiers jusqu'au fichier voulu (voir le tableau ci-dessous).
3. Cliquez sur l'icône **crayon** (*Edit this file*), en haut à droite du fichier.
4. Corrigez ou ajoutez votre texte.
5. Cliquez sur le bouton vert **Commit changes…**, puis encore sur **Commit changes**.
6. Attendez quelques minutes et rechargez votre site.

Une erreur ? Le site ne se met simplement pas à jour (croix rouge dans l'onglet *Actions*) : l'ancienne version reste en ligne.
Ouvrez à nouveau le fichier, corrigez, et enregistrez.

## Où se trouve chaque texte

Les dossiers `fr`, `ar` et `en` contiennent les trois langues : **pensez à corriger les trois versions**.

| Ce que vous voulez modifier | Fichier |
|---|---|
| Votre titre, biographie, domaines de recherche | `data/authors/me.yaml` (français), `data/ar/authors/me.yaml`, `data/en/authors/me.yaml` |
| Diplômes (rubrique *education*) | même fichier `me.yaml` |
| Expériences professionnelles (rubrique *experience*) | même fichier `me.yaml` |
| Texte « Mes recherches » et chiffres clés de l'accueil | `content/fr/_index.md` |
| Formations complémentaires, langues | `content/fr/parcours/index.md` |
| Une publication | `content/fr/publications/NOM-DU-DOSSIER/index.md` |
| Communications et séminaires | `content/fr/communications/index.md` |
| Un projet | `content/fr/projets/NOM-DU-DOSSIER/index.md` |
| Enseignement | `content/fr/enseignement/index.md` |
| Une réflexion (article de blog) | `content/fr/reflexions/NOM-DU-DOSSIER/index.md` |
| Votre photo | `assets/media/authors/me.png` (bouton *Add file > Upload files* pour la remplacer, même nom) |

## Les 3 règles à respecter

Les fichiers commencent par un en-tête entre deux lignes `---`. Dans cet en-tête :

1. **Gardez l'alignement** (les espaces en début de ligne) exactement comme dans les lignes voisines.
2. **Ne supprimez pas les guillemets** autour d'un texte qui en a.
3. **Ne touchez pas aux mots avant les deux-points** (`title:`, `role:`, `start:`…) : changez seulement ce qui vient après.

Sous l'en-tête, le texte est libre : écrivez normalement. `**mot**` met en **gras**, une ligne commençant par `- ` crée une liste.

## Exemples

### Ajouter une expérience (dans `me.yaml`, rubrique `experience:`)

Copiez un bloc existant et collez-le juste en dessous, puis modifiez-le :

```yaml
- role: Membre du comité scientifique
  org: Revue XYZ, Université Alger 3
  start: '2026-01-01'
  summary: Évaluation des articles soumis.
```

Sans ligne `end:`, l'expérience s'affiche « Actuellement ». Avec `end: '2026-06-30'`, elle s'affiche terminée.

### Ajouter une communication (dans `content/fr/communications/index.md`)

Ajoutez une ligne dans la liste, en gardant les 8 espaces au début :

```
        - **Mars 2026** – Communication « Titre », colloque « Nom du colloque », Université …, 12 mars 2026.
```

### Ajouter un article scientifique

1. Ouvrez `content/fr/publications/`, puis un dossier d'article existant, puis `index.md`.
2. Copiez tout son contenu.
3. Revenez à `content/fr/publications/`, cliquez sur *Add file > Create new file* et nommez le fichier
   `nom-court-de-l-article/index.md` (le `/` crée le dossier).
4. Collez, remplacez le titre, la date, la revue (`publication: name:`), le résumé, puis enregistrez.
5. Pour ajouter un lien vers le PDF ou la page de la revue, remplacez `links: []` par :

```yaml
links:
  - type: pdf
    url: https://www.asjp.cerist.dz/...
```

### Écrire une nouvelle réflexion

Même méthode : copiez `content/fr/reflexions/bienvenue/index.md` dans un nouveau dossier
(ex. `content/fr/reflexions/pouvoir-achat-2026/index.md`), puis changez le titre, la date, le résumé et le texte.
Pour la version arabe ou anglaise, créez un dossier **du même nom** dans `content/ar/reflexions/` ou `content/en/reflexions/`.

## Besoin d'aide ?

Vous pouvez aussi m'envoyer vos corrections (texte, CV mis à jour, photos) : je les intègre et je vous renvoie le site à jour.
