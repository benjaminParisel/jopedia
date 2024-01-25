# Construction de JOpedia

## Objectif

A la suite de ces steps, nous allons constuire un rendu similaire à [ce mini site](https://benjaminparisel.github.io/jopedia/).

## Common step

Pour visualiser correctement le rendu du site, nous allons utiliser `http-server`.

Dans un terminal séparé, à la racine de ce repository, lancer `npm run build:serve` (et veillez à bien le garder constamment actif).
Pour générer le site, utiliser la commande `npm run build:dev`

## Etape 3: Aggrégation de plusieurs composants

Modifier le fichier `antora-playbook.yml` pour ajouter 2 extensions:

### AsciiDoc

Intégration de [Asciidoctor Kroki Extension](https://github.com/asciidoctor/asciidoctor-kroki)

> npm i --save-dev @antora/lunr-extension

```
asciidoc:
  attributes:
    kroki-fetch-diagram: true
  extensions:
    - asciidoctor-kroki
```
- Regénérer le site et aller sur [http://localhost:8080/summer/2020/medals](http://localhost:8080/summer/2020/medals)
### Antora

Intégration de [Antora-Lunr-extensions](https://gitlab.com/antora/antora-lunr-extension)

> npm i --save-dev @antora/lunr-extension

- Modifier le fichier `antora-playbook.yml`pour ajouter:

```
 antora:
  extensions:
    - '@antora/lunr-extension'
```

- Regénerer le site et rafraichir [http://localhost:8080/](http://localhost:8080/)

## Etape suivante

La suite se trouve sur la branche: step/4-ui
