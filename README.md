# Construction de JOpedia

## Objectif

A la suite de ces steps, nous allons constuire un rendu similaire à [ce mini site](https://benjaminparisel.github.io/jopedia/).

## Common step

Pour visualiser correctement le rendu du site, nous allons utiliser `http-server`.

Dans un terminal séparé, à la racine de ce repository, lancer `npm run build:serve` (et veillez à bien le garder constamment actif).

Pour générer le site, utiliser la commande `npm run build:dev`.

## Etape 4: Amélioration de l'UI

Utilisez [ui-supplemental](https://docs.antora.org/antora/latest/playbook/ui-supplemental-files/) pour:

- Modifier l'icone dans l'onglet du navigateur

- Supprimer les boutons statiques récupérer dynamiquement le titre des composants pour les afficher dans le header.

Tips:

- Structure de la [UI par défaut](https://gitlab.com/antora/antora-ui-default/-/tree/master/src?ref_type=heads) fournie par Antora
- Le fichier svg de l'icone à ajouter est fournie dans le dossier `./filesToMove`

## Etape suivante et correction

La suite se trouve sur la branche: step/5-xxx
