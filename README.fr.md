Ce README est en français. [Lire en anglais](README.md)

# CalmCSS

**CalmCSS** est une base CSS minimaliste, sans classes et accessible, conçue pour démarrer rapidement des projets web clairs et naturels. Cette feuille de style repose uniquement sur des éléments HTML5 sémantiques et des variables CSS modernes pour fournir une fondation solide sans surcharge de classes ou de frameworks.

---

## Fonctionnalités clés

* **CSS sans classes** : Styles basés uniquement sur les balises HTML5.
* **Variables CSS** : Couleurs, typographie, espacements et transitions configurables.
* **Mode sombre automatique** : S’adapte aux préférences système de l’utilisateur.
* **Design accessible** : Polices lisibles, contrastes optimisés, responsive.
* **Menu mobile adaptatif** : Menu simple utilisant `<details>` et `<summary>`, sans JavaScript.
* **Structure modulaire** : Fichiers séparés pour styles de base et composants de mise en page.
* **Polyvalent** : Convient pour petits projets, prototypes ou bases de sites complets.

---

## Installation

Téléchargez simplement le fichier `calm.css` et liez-le à votre projet HTML :

```html
<link rel="stylesheet" href="calm.css" />
```

Un layout centré avec largeur maximale est inclus par défaut via :

```css
@import "layout-center-container.css";
```

Aucun paramétrage supplémentaire n’est nécessaire.

---

## Utilisation

Incluez CalmCSS dans la balise `<head>` de votre document HTML. La feuille de style stylise automatiquement tous les éléments HTML5 sans ajouter de classes.

Exemple minimal :

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <title>Projet avec CalmCSS</title>
    <link rel="stylesheet" href="calm.css" />
  </head>
  <body>
    <header><h1>Bienvenue sur mon site</h1></header>
    <main>
      <p>Un simple paragraphe stylisé naturellement.</p>
    </main>
  </body>
</html>
```

---

## Menu déroulant mobile

CalmCSS inclut maintenant un **menu mobile en CSS pur** utilisant `<details>` et `<summary>`. Aucun JavaScript n’est requis.

Exemple :

```html
<nav>
  <ul>
    <li><a href="#typography">Typographie</a></li>
    <li><a href="#forms">Formulaires</a></li>
    <li><a href="#tables">Tables</a></li>
    <li><a href="#code">Code</a></li>
    <li><a href="#media">Médias</a></li>
  </ul>

  <!-- Navigation mobile -->
  <details>
    <summary>Menu</summary>
    <ul>
      <li><a href="#typography">Typographie</a></li>
      <li><a href="#forms">Formulaires</a></li>
      <li><a href="#tables">Tables</a></li>
      <li><a href="#code">Code</a></li>
      <li><a href="#media">Médias</a></li>
    </ul>
  </details>
</nav>
```

Le comportement adaptatif est automatique via les media queries :

* Desktop : navigation horizontale affichée.
* Mobile (≤768px) : navigation desktop masquée, menu `<details>` affiché.

---

## Personnalisation

Modifiez les variables CSS dans `:root` pour adapter les couleurs, la typographie, les espacements et les transitions.

---

## Contribuer

Les contributions, corrections et suggestions sont les bienvenues ! Veuillez ouvrir un issue ou un pull request.

---

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
