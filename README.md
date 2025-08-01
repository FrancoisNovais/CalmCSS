# CalmCSS

**CalmCSS** is a minimalist, class-free, and accessible CSS base designed to help you quickly start clear and natural web projects. This stylesheet relies solely on semantic HTML5 elements and modern CSS variables to provide a solid foundation without any class or framework overhead.

---

## Key Features

- **Classless CSS**: Styling based purely on native HTML5 tags.
- **CSS Variables**: Configurable colors, typography, spacing, and transitions.
- **Automatic Dark Mode**: Adapts to user’s system preferences.
- **Accessible Design**: Readable fonts, well-considered contrasts, responsive.
- **Responsive**: Simple mobile-friendly dropdown menu with minimal setup.
- **Modular Structure**: Separate files for base styles and layout components.
- **Versatile**: Suitable for small projects, prototypes, or as a base for full websites.

---

## Installation

Simply download the `calm.css` file and link it in your HTML project :

```html
<link rel="stylesheet" href="calm.css" />
```

A centered layout with maximum width is **included by default** in CalmCSS via :

```css
@import "layout-center-container.css";
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

## Mobile Dropdown Menu (optional)

Because perfection is hard to reach, CalmCSS includes a simple `.open` class and a small JavaScript snippet to enable a mobile-friendly dropdown menu without complicating the base CSS.

> Note: This feature is **enabled by default** in the included layout CSS file (`layout-center-container.css`).  
> You just need to add the JavaScript snippet into your HTML.

```html
<script>
  document.addEventListener("DOMContentLoaded", () => {
    const nav = document.querySelector("nav");
    nav.addEventListener("click", () => {
      if (window.innerWidth <= 768) {
        nav.classList.toggle("open");
      }
    });
  });
</script>
```

This snippet toggles the `.open` class on the `<nav>` element when clicked on screens 768px wide or less, enabling a simple toggle menu.

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
