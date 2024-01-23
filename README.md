# Construction de JOpedia

## Objectif

A la suite de ces steps, nous allons constuire un rendu similaire à [ce mini site](https://benjaminparisel.github.io/jopedia/).

## Common step

Pour visualiser correctement le rendu du site, nous allons utiliser `http-server`.

Dans un terminal séparé, à la racine de ce repository, lancer `npm run build:serve` (et veillez à bien le garder constamment actif).

Pour générer le site, utiliser la commande `npm run build:dev`.

## Etape 6: Redirect

Pour éviter les liens morts (les 404 c'est pas beau), un attribut `:page-aliases:` est disponible et à mettre dans le header des pages de contenu. Lors d'une suppression ou d'un changement d'organisation d'une page il est recommandé d'ajouté cette attribut.

- Dans les sources du contenu de `jo-summer`, regarder le fichier XXXXX
- Depuis le site généré lors de l'étape précédente (ou `npm run build:dev`), copier et coller cette url [http://localhost:8080/summer/xxxxxx](http://localhost:8080/summer/xxxxxx)
- Une redirection est effectuée et la page afficher est "Titre de la page à choisir"

Docs:

- [page-aliases](https://docs.antora.org/antora/latest/page/page-aliases/)

## Etape suivante et correction

Félicitation, votre mini site sur le thème des Jeux olympiques est prêt et ressemble grandement à l'objectif fixé.

Si vous souhaitez allez plus loin avec Antora, la documentation officielle est là pour vous.
