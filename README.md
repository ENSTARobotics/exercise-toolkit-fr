# Exercise Toolkit FR

Version française légère du moteur pédagogique utilisé par les exercices GitHub Skills.

Ce dépôt fournit les workflows réutilisables et les templates génériques nécessaires pour construire des exercices interactifs en français, sans générer d'abord des messages en anglais puis les remplacer.

## Workflows réutilisables

- `.github/workflows/start-exercise.yml` : initialise l'exercice, crée l'Issue de cours et met à jour le README.
- `.github/workflows/find-exercise-issue.yml` : retrouve l'Issue de l'exercice.
- `.github/workflows/finish-exercise.yml` : publie le message final, met à jour le README et ferme l'Issue.

## Templates

Les textes génériques sont dans `markdown-templates/` et sont produits directement en français.

Les contenus propres à chaque cours restent dans le dépôt du cours, par exemple `.github/steps/`.

## Origine

Ce projet est adapté de [skills/exercise-toolkit](https://github.com/skills/exercise-toolkit), distribué sous licence MIT.

L'objectif est de conserver l'expérience et l'architecture GitHub Skills tout en offrant une interface française native.
