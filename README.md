# WikiHome

La documentation technique de la vie domestique. Concise. Structuree. Sans blabla.

**[Consulter le site](https://vblackjack.github.io/WikiHome/)**

## Concept

WikiHome est une base de connaissances "No-Fluff" pour la gestion efficace du quotidien. Chaque article suit une structure standardisee :

**Prerequis > Etapes numerotees > Depannage**

Pas de narration, pas d'anecdotes, pas de blabla. Juste l'information actionnable.

## Contenu

### Cuisine (25 articles)

**Fondamentaux** — Comprendre les ingredients et le materiel avant de cuisiner.

- Beurre : appellations, cuisson et clarification
- Huile d'olive : appellations, extraction et degustation
- Qualite des oeufs : codes d'elevage, oeufs de cane
- Materiaux et revetements des ustensiles de cuisson
- Techniques anti-adherence (acier carbone, inox)
- Mythes en cuisine : vrai ou faux (30+ mythes documentes)
- Conservation des aliments : DLC, DDM, congelation
- Equivalences et conversions (volumes, poids, substitutions)

**Techniques de base** — Les gestes essentiels.

- Cuisson des oeufs (coque, mollet, dur)
- Cuisson du riz : 4 methodes comparees
- Cuisson des viandes : temperatures a coeur, repos, reverse sear
- Pomme de terre : varietes, cuissons et conservation
- Sauces de base : vinaigrette, sauce tomate, fond de volaille
- Les 4 pates a tarte (brisee, sablee, sucree, feuilletee)
- Pate a crepes et impact du repos

**Recettes** — Procedures completes et testees.

- Crepes Raymond Oliver (1954)
- Crepes Paul Bocuse (beurre noisette)
- Puree Joel Robuchon
- Lasagnes alla Bolognese (tradition)
- Pain au levain naturel
- Pancakes au surplus de levain
- Rouleaux de printemps vietnamiens (Goi Cuon)
- Bi Cuon (porc et poudre de riz grille)

### Bricolage (3 articles)

- Chevilles et fixations : choisir selon le support
- Purger un radiateur
- Changer un joint (robinet, siphon, chasse d'eau)

### Saisonnier (4 articles)

- Montage du sapin de Noel (technique pro)
- Specifications techniques du sapin
- Checklist vacances : fermeture du domicile
- Entretien saisonnier du domicile

### Admin (1 article)

- Checklist administrative annuelle (echeances, durees de conservation)

## Fonctionnalites

| Fonctionnalite | Detail |
| :--- | :--- |
| Theme | Dracula (sombre/clair avec toggle) |
| Navigation | Onglets, sous-sections, chargement instantane |
| Recherche | Suggestions, surlignage, separateur francais |
| Tags | Filtrage par theme (debutant, technique, recette, viande, vegetarien...) |
| Depannage | Sections collapsibles sur chaque article |
| Liens croises | Navigation entre articles connexes |
| Checkboxes | Listes d'ingredients et de materiel interactives |

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
    tags.md
    404.md
    stylesheets/
      dracula.css
    guides/
      cuisine/
        index.md
        beurre.md
        ...
      bricolage/
        index.md
        chevilles_fixations.md
        ...
      saisonnier/
        index.md
        montage_sapin.md
        ...
      admin/
        index.md
        checklist_administrative.md
  _templates/
    guide_type.md
  mkdocs.yml
```

## Contribuer

Chaque article doit respecter le template `_templates/guide_type.md` :

1. Frontmatter YAML (tags)
2. Metadonnees (date, duree, difficulte)
3. Materiel / Ingredients (checklist)
4. Procedure (etapes numerotees)
5. Depannage / FAQ (tableau collapsible `??? note`)
6. Notes (admonitions MkDocs)
7. Liens croises (`Voir aussi`)

## Licence

Copyright 2026 Julien Bombled

Licensed under the Apache License, Version 2.0.
