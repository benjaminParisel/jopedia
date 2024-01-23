# Construction de JOpedia

## Objectif

A la suite de ces steps, nous allons constuire un rendu similaire à [ce mini site](https://benjaminparisel.github.io/jopedia/).

## Common step

Pour visualiser correctement le rendu du site, nous allons utiliser `http-server`.

Dans un terminal séparé, à la racine de ce repository, lancer `npm run build:serve` (et veillez à bien le garder constamment actif).

Pour générer le site, utiliser la commande `npm run build:dev`

## Etape 5: Urls

Avec Antora, il est possible out-of-the box de gérer des URLs unique pour la version latest et pour la prochaine version à venir.
Ces modifications se situe à un seul endroit, encore et toujours le `antora-playbook.yml`.

### Latest

A la suite du playbook, ajouter la clé suivante:

```
urls:
    latest_version_segment: <Replace_with_any_value>
    latest_version_segment_strategy: redirect:to
```

Une fois la modification effectué et le site regénérer, comparer dans un nouvel onglet l'url affichée dans le browser.

### Next

Pour le composant `jo-summer` ajouter la branche `2024`, et la branche `2026` pour le composant `jo-winter`.

Dans le fichier de configuration de la version 2024, le champs [prerelease](https://github.com/benjaminParisel/jo-summer/blob/2024/docs/antora.yml#L4) est utilisé pour déclarer cette version comme future.

Puis dans le fichier playbook ajouter la clé pour l'entrée `urls` créée précedement.

```
    latest_prerelease_version_segment: <Replace_with_any_value>
```

Tips:

- Utiliser [latest-version-segment](https://docs.antora.org/antora/latest/playbook/urls-latest-version-segment/)
- Utiliser [latest_prerelease_version_segment](https://docs.antora.org/antora/latest/playbook/urls-latest-prerelease-version-segment/)

## Etape suivante et correction

La suite se trouve sur la branche: step/6-redirect
