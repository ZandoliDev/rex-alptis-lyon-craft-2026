# REX Lyon Craft — Didier & Laure

Repo de travail collaboratif pour la préparation du talk REX à Lyon Craft.

**[Voir la présentation en ligne](https://zandolidev.github.io/rex-alptis-lyon-craft-2026/)**

## Organisation

```
contenu/    → tous les fichiers markdown (trame, plan, discours…)
support/    → le support de présentation (reveal-md)
CLAUDE.md   → contexte projet pour Claude Code
```

## Travailler avec Claude Code

Depuis la racine du repo :

```bash
claude
```

Claude Code lit automatiquement `CLAUDE.md` et a accès à tout le contexte du projet.

## Présentation (reveal-md)

Le support est un fichier Markdown (`support/REX_Lyon_Craft.md`) transformé en présentation HTML par [reveal-md](https://github.com/webpro/reveal-md).

```bash
npm install        # installer les dépendances
npm start          # lancer en mode dev (http://localhost:1948, hot-reload) — sert tout le dossier support/
npm run build      # générer la version statique dans support/dist/
```

En mode dev, la touche `S` ouvre les **speaker notes**.

Les slides sont séparés par `---`. Les notes orales s'ajoutent avec `Note:` sous chaque slide.

Il est possible de découper la présentation en plusieurs fichiers `.md` (par exemple un par acte). En lançant `npx reveal-md support/`, reveal-md affiche une page d'index listant tous les fichiers Markdown du dossier, chacun devenant une présentation navigable indépendamment.

## Étapes en cours

Voir `contenu/REX_Lyon_Craft_Plan_Action.md` pour le statut de chaque étape.

## Conventions Git

- Commits en français
- Format : `type: description courte`
- Types : `feat` (nouveau livrable), `fix` (correction), `refactor` (réécriture)
