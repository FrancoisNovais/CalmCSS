This README is in English. [Read in French](README.fr.md)

# CalmCSS

**CalmCSS** is a minimalist, class-free, and accessible CSS base designed to help you quickly start clear and natural web projects. This stylesheet relies solely on semantic HTML5 elements and modern CSS variables to provide a solid foundation without any class or framework overhead.

---

## Key Features

- **Classless CSS**: Styling based purely on native HTML5 tags.
- **CSS Variables**: Configurable colors, typography, spacing, and transitions.
- **Automatic Dark Mode**: Adapts to user’s system preferences.
- **Accessible Design**: Readable fonts, well-considered contrasts, responsive.
- **Responsive**: Simple mobile-friendly dropdown menu using native `<details>` and `<summary>`.
- **Modular Structure**: Separate files for base styles and layout components.
- **Versatile**: Suitable for small projects, prototypes, or as a base for full websites.

---

## Installation

Simply download the `calm.css` file and link it in your HTML project :

```html
<link rel="stylesheet" href="calm.css" />
```

A centered layout with maximum width is **included by default** in CalmCSS via :

```html
  <style>
    @import url("../css/layouts/layout-center-container.css");
  </style>
```

So no additional setup is required.

---

## Usage

Include CalmCSS in the `<head>` of your HTML document.  
The stylesheet automatically styles all HTML5 elements without the need to add classes.

Minimal example:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Project with CalmCSS</title>
    <link rel="stylesheet" href="calm.css" />
  </head>
  <body>
    <header><h1>Welcome to my site</h1></header>
    <main>
      <p>A simple paragraph styled naturally.</p>
    </main>
  </body>
</html>
```

---

## Mobile Dropdown Menu

CalmCSS now includes a **pure CSS mobile dropdown menu** using `<details>` and `<summary>`. No JavaScript is required.

Example:

```html
<nav>
  <ul>
    <li><a href="#typography">Typography</a></li>
    <li><a href="#forms">Forms</a></li>
    <li><a href="#tables">Tables</a></li>
    <li><a href="#code">Code</a></li>
    <li><a href="#media">Media</a></li>
  </ul>

  <!-- Mobile navigation -->
  <details>
    <summary>Menu</summary>
    <ul>
      <li><a href="#typography">Typography</a></li>
      <li><a href="#forms">Forms</a></li>
      <li><a href="#tables">Tables</a></li>
      <li><a href="#code">Code</a></li>
      <li><a href="#media">Media</a></li>
    </ul>
  </details>
</nav>
```

Responsive behavior is automatic via media queries:

* Desktop: horizontal nav is displayed.
* Mobile (≤48rem): desktop nav is hidden, and `<details>` menu is shown.

---

## Customization

Modify the CSS variables inside `:root` to adapt colors, typography, spacing, and transitions to your needs.

---

## Contributing

Contributions, fixes, and suggestions are welcome!  
Please open an issue or a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
