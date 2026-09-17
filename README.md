# grind

## Contenu actuel

- [`index.html`](index.html) — page d'accueil basique
- [`hello-quentin.html`](hello-quentin.html) — page de test
- [`prospection.html`](prospection.html) — maquette de l'outil de prospection restaurant (recherche par ville + scoring, données factices pour l'instant)

## Workflow Git

- `main` : toujours stable, c'est la branche de référence.
- `arthur` : branche de travail d'Arthur.
- `quentin` : branche de travail de Quentin.

Chacun commit sur sa propre branche, puis merge dans `main` (idéalement via une Pull Request GitHub pour permettre une relecture avant merge) :

```bash
git checkout ma-branche
git add .
git commit -m "message clair"
git push origin ma-branche
# puis ouvrir une PR sur GitHub vers main
```

Avant de commencer une nouvelle tâche, pense à récupérer les derniers changements de `main` :

```bash
git checkout ma-branche
git merge main
```

## Setup local

Aucune dépendance pour l'instant (pages HTML statiques). Si le projet passe à Node :

```bash
npm install
```

Le `.gitignore` est déjà prêt pour ça (`node_modules/`, `.env`, `dist/`, etc.).
