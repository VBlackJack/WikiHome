# WikiHome

La documentation technique de la vie domestique. Concise. Structuree. Sans blabla.

**[Consulter le site](https://vblackjack.github.io/WikiHome/)**

## Concept

WikiHome est une base de connaissances "No-Fluff" pour la gestion efficace du quotidien. Chaque article suit une structure standardisee :

**Prerequis > Etapes numerotees > Depannage**

Pas de narration, pas d'anecdotes, pas de blabla. Juste l'information actionnable.

## Contenu

### Cuisine

**Fondamentaux** — Comprendre les ingredients et le materiel avant de cuisiner.

- Beurre : appellations, cuisson et clarification
- Huile d'olive : appellations, extraction et degustation
- Qualite des oeufs : codes d'elevage, oeufs de cane
- Materiaux et revetements des ustensiles de cuisson
- Techniques anti-adherence (acier carbone, inox)
- Mythes en cuisine : vrai ou faux (30+ mythes documentes)

**Techniques de base** — Les gestes essentiels.

- Cuisson des oeufs (coque, mollet, dur)
- Cuisson du riz : 4 methodes comparees
- Pomme de terre : varietes, cuissons et conservation
- Les 4 pates a tarte (brisee, sablee, sucree, feuilletee)
- Pate a crepes et impact du repos

**Recettes** — Procedures completes et testees.

- Crepes Raymond Oliver (1954)
- Crepes Paul Bocuse (beurre noisette)
- Puree Joel Robuchon
- Lasagnes alla Bolognese (tradition)
- Pancakes au surplus de levain
- Rouleaux de printemps vietnamiens (Goi Cuon)
- Bi Cuon (porc et poudre de riz grille)

### Saisonnier

- Montage du sapin de Noel (technique pro)
- Specifications techniques du sapin

## Stack technique

| Composant | Technologie |
| :--- | :--- |
| Generateur | [MkDocs](https://www.mkdocs.org/) |
| Theme | [Material for MkDocs](https://squidfdev.github.io/mkdocs-material/) + Dracula |
| Deploiement | GitHub Pages (CI automatique via GitHub Actions) |
| Format | Markdown |

## Developpement local

```bash
pip install mkdocs-material
mkdocs serve
```

Le site est accessible sur `http://127.0.0.1:8000`.

## Structure du projet

```
WikiHome/
  docs/
    index.md
    stylesheets/
      dracula.css
    guides/
      cuisine/
        index.md
        beurre.md
        ...
      saisonnier/
        index.md
        montage_sapin.md
        ...
  _templates/
    guide_type.md
  mkdocs.yml
```

## Contribuer

Chaque article doit respecter le template `_templates/guide_type.md` :

1. Metadonnees (date, duree, difficulte)
2. Materiel / Ingredients (checklist)
3. Procedure (etapes numerotees)
4. Depannage / FAQ (tableau collapsible)
5. Notes (admonitions MkDocs)

## Licence

Copyright 2026 Julien Bombled

Licensed under the Apache License, Version 2.0.
