# Site de cours — STT-2902

Site du cours STT-2902 Modélisation statistique (baccalauréat en enseignement au secondaire, mathématiques) : accueil, plan de cours, calendrier, liens avec le programme du secondaire, activités et projet SAÉ, générés avec [Quarto](https://quarto.org).

Le cours tient compte des nouveaux préalables STT-1300 et STT-1500 : la statistique descriptive, l'échantillonnage et l'estimation ne sont plus refaits, et le temps libéré sert à relier chaque méthode à deux variables au programme de mathématique du secondaire.

## Développement local

```bash
quarto preview          # prévisualise le site
quarto render --to html # génère le site dans _site/
```

## Publication

Chaque push sur `main` déclenche `.github/workflows/publish.yml`, qui rend le site et le publie sur GitHub Pages. Dans les réglages du dépôt, *Settings → Pages → Source* doit être réglé sur « GitHub Actions ».

## Structure

```
.
├── _quarto.yml            # configuration du site
├── index.qmd              # accueil
├── plan-de-cours.qmd      # préalables, objectifs, principes, évaluation, références
├── calendrier.qmd         # les 15 semaines
├── secondaire.qmd         # liens entre le programme du secondaire et le cours
├── activites.qmd          # activités (Mayer, rectangle, écart moyen, dépistage, Simpson…)
├── projet.qmd             # projet SAÉ
├── styles.css             # thème commun aux sites de cours (copié de STT-7360)
├── date-modification-bas-page.html
└── images/nuage.svg       # illustration de l'accueil et favicon
```
