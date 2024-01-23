# Construction de JOpedia

## Objectif

A la suite de ces steps, nous allons constuire un rendu similaire à [ce mini wiki](https://benjaminparisel.github.io/jopedia/)

## Common step

Pour visualiser correctement le rendu du site, nous allos utiliser `http-server`
Dans un terminal séparé, à la racine de ce repository, lancer `npm run build:serve` (et veillez à bien le garder constamment actif)

## Etape 2: Aggrégation de plusieurs composants

Modifier le fichier `antora-playbook.yml` pour:

- Afficher comme titre `JOpedia`
- Aggréger les 2 composants:
  ** https://github.com/benjaminParisel/jo-summer, les branches 2016,2020
  ** https://github.com/tbouffard/jo-winter, les branches 2018,2022

Run `npm run build:dev` puis accédez à [http://localhost:8080/](http://localhost:8080/)

- Faire en sorte que l'utilisateur soit rediriger sur la page d'accueil des JO d'été

## Etape suivante

La suite se trouve sur la branche: step/3-ui
