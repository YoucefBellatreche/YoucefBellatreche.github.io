# Site personnel – Dr Youcef Bellatreche

Site trilingue (français, arabe, anglais) construit avec **Hugo Blox** (modèle *Academic CV*).

## 0. Voir le site avant de le mettre en ligne

Décompressez `apercu-site-bellatreche.zip`, ouvrez le dossier obtenu et double-cliquez sur `index.html` :
le site s'ouvre dans votre navigateur, sans connexion Internet ni installation.
(La recherche interne ne fonctionne qu'une fois le site en ligne.)

## Hébergement : gratuit

GitHub Pages est gratuit pour un dépôt public avec un compte GitHub Free
(documentation officielle : https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages).
Seul un nom de domaine personnel (ex. `bellatreche.dz` ou `.com`) serait payant, et il est facultatif.

## 1. Mettre le site en ligne (gratuit, GitHub Pages)

1. Créez un compte sur https://github.com (bouton *Sign up*).
2. Installez **GitHub Desktop** (https://desktop.github.com) et connectez-vous avec ce compte.
3. Dans GitHub Desktop : *File > New repository*.
   - **Name** : `VOTRE-IDENTIFIANT.github.io` (remplacez par votre identifiant GitHub, en minuscules).
     Votre site aura alors l'adresse `https://VOTRE-IDENTIFIANT.github.io`.
   - Cliquez sur *Create repository*.
4. Cliquez sur *Show in Finder*, puis copiez **tout le contenu** du dossier `site-bellatreche` dans ce dossier
   (y compris le dossier caché `.github` : dans le Finder, appuyez sur `Cmd + Maj + .` pour afficher les fichiers cachés).
5. Revenez dans GitHub Desktop : écrivez un résumé (ex. « Première version »), cliquez sur *Commit to main*, puis sur *Publish repository*
   (**décochez** *Keep this code private*).
6. Sur github.com, ouvrez le dépôt : *Settings > Pages > Build and deployment > Source* : choisissez **GitHub Actions**.
7. Onglet *Actions* : attendez que le déploiement passe au vert (2 à 5 minutes). Le site est en ligne.

Chaque modification envoyée ensuite (*Commit* puis *Push origin*) met le site à jour automatiquement.

## 2. Où modifier quoi

➡️ Le mode d'emploi détaillé, avec exemples, est dans **GUIDE-MODIFIER-LE-SITE.md**.

| Élément | Fichier |
|---|---|
| Profil, biographie, formation, expériences, compétences (français) | `data/authors/me.yaml` |
| Même chose en arabe / en anglais | `data/ar/authors/me.yaml`, `data/en/authors/me.yaml` |
| Photo de profil | `assets/media/authors/me.png` (remplacez-la par une photo carrée d'au moins 600 × 600 pixels) |
| Page d'accueil | `content/fr/_index.md` (et `content/ar/`, `content/en/`) |
| Publications | `content/fr/publications/` : un dossier par publication |
| Communications (colloques, séminaires) | `content/fr/communications/index.md` |
| Projets et responsabilités | `content/fr/projets/` (image de couverture : `featured.png` dans chaque dossier) |
| Couleurs et animations | `assets/css/custom.css` |
| Enseignement | `content/fr/enseignement/index.md` |
| Réflexions (blog) | `content/fr/reflexions/` |
| Menus et langues | `config/_default/languages.yaml` |
| Nom du site, couleurs principales | `config/_default/params.yaml` |

## 3. Publier une nouvelle réflexion

Copiez le dossier `content/fr/reflexions/bienvenue`, renommez-le (ex. `pouvoir-achat-2026`), puis modifiez `index.md` :

```markdown
---
title: Titre de l'article
summary: Une phrase de résumé.
date: 2026-11-05
authors:
  - me
tags:
  - Économie algérienne
---

Texte de l'article…
```

Pour la version arabe ou anglaise, créez un dossier **du même nom** dans `content/ar/reflexions/` ou `content/en/reflexions/` :
le sélecteur de langue reliera automatiquement les deux versions.

## 4. Ajouter un article scientifique

Copiez `content/fr/publications/memoire-dea`, renommez le dossier, puis adaptez :
`title`, `date`, `publication_types` (`article-journal` pour un article de revue, `paper-conference` pour une communication,
`chapter` pour un chapitre d'ouvrage), `publication.name` (nom de la revue) et `links` (lien PDF ou DOI).

## 5. Prévisualiser sur votre ordinateur (facultatif)

Installez Hugo extended 0.162.0, Go et Node.js (pnpm), puis : `pnpm install` et `hugo server`.
