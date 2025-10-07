Ce CHANGELOG est en français. [Read in English](CHANGELOG.md)

# Journal des modifications

Tous les changements notables de ce projet seront documentés dans ce fichier.

Le format est basé sur [Keep a Changelog](https://keepachangelog.com/fr/1.0.0/).

## [Non publié]

### Ajouté
- Version initiale de CalmCSS
- Base CSS sans classes avec support HTML5 sémantique
- Mode sombre automatique basé sur les préférences système de l'utilisateur
- Variables CSS pour une personnalisation facile (couleurs, typographie, espacements, transitions)
- Layout responsive avec conteneur centré
- Navigation mobile utilisant les éléments natifs `<details>` et `<summary>`
- Styles complets pour les formulaires, tableaux, blocs de code et typographie
- Fonctionnalités d'accessibilité incluant le support du mode contraste élevé
- Styles adaptés pour l'impression
- Architecture modulaire avec fichiers de mise en page séparés
- Licence MIT

### Modifié
- **Navigation mobile refactorisée de JavaScript vers HTML natif** : Remplacement du menu mobile dépendant de JavaScript par une solution CSS pure utilisant les éléments `<details>` et `<summary>`
- Breakpoint mobile standardisé à 48rem (768px) dans tous les fichiers
- Ajout de variables CSS pour les breakpoints : `--breakpoint-mobile` et `--breakpoint-desktop`
- Amélioration de la structure du projet avec des répertoires dédiés

### Corrigé
- Unification des breakpoints responsive pour utiliser les unités rem de manière cohérente
- Suppression des media queries conflictuelles entre calm.css et layout-center-container.css
- Élimination du code obsolète du menu mobile qui référençait une classe `.open` inexistante
- Correction des valeurs de breakpoint incohérentes (40rem vs 768px)

### Fonctionnalités
- Approche sans classes - fonctionne immédiatement avec du HTML simple
- Aucune dépendance JavaScript pour la navigation mobile
- Meilleure accessibilité avec l'élément natif `<details>` (navigation au clavier, support des lecteurs d'écran)
- Layouts modernes avec CSS Grid et Flexbox
- Transitions et animations fluides
- Code plus propre sans couplage JavaScript