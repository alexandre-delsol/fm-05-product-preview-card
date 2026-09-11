# Frontend Mentor — Product Preview Card Component

A responsive product preview card built as part of the [Frontend Mentor](https://www.frontendmentor.io/) challenges.

The goal of this challenge was to reproduce the provided design as accurately as possible while strengthening my fundamentals in **HTML and CSS**, particularly responsive layouts, Flexbox, typography, and semantic HTML.

## 📸 Overview

### The challenge

Users should be able to:

* View the optimal layout depending on their device's screen size.
* See hover and focus states for interactive elements.
* View the product information and pricing clearly.
* Interact with the "Add to Cart" button.

### Screenshot

*Add your final screenshot here if you want to showcase the result.*

## 🛠️ Built with

* Semantic HTML5
* CSS3
* Flexbox
* CSS custom properties
* Responsive design
* `<picture>` and `<source>` for responsive images
* Google Fonts

  * Montserrat
  * Fraunces

## 📚 What I learned

This challenge allowed me to reinforce several frontend fundamentals.

### Responsive images

I used the `<picture>` element to display a different image depending on the viewport width:

```html
<picture>
    <source media="(max-width: 600px)" srcset="./images/image-product-mobile.jpg">
    <img src="./images/image-product-desktop.jpg" alt="Gabrielle Essence Eau De Parfum">
</picture>
```

This was useful for understanding that responsive design is not limited to resizing an image with CSS: sometimes the appropriate solution is to provide a different image asset.

### Flexbox

The component uses Flexbox for both the main layout and the button:

```css
main {
    display: flex;
}

button {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
}
```

I reinforced my understanding of:

* `flex-direction`
* `justify-content`
* `align-items`
* `gap`
* main and cross axes


### CSS custom properties

I used CSS variables to centralize the main colors:

```css
:root {
    --color-light-green: hsl(158, 36%, 37%);
    --color-dark-green: hsl(158, 42%, 18%);
    --color-black: hsl(212, 21%, 14%);
    --color-grey: hsl(228, 12%, 48%);
    --color-cream: hsl(30, 38%, 92%);
    --color-white: hsl(0, 0%, 100%);
}
```

This makes the stylesheet easier to maintain and keeps repeated values consistent.

### Accessibility basics

The cart icon is decorative, so it uses an empty `alt` attribute:

```html
<img src="./images/icon-cart.svg" alt="">
```

The "Add to Cart" action uses a semantic `<button>` rather than a link because it represents an action.

## 🧠 Challenges and decisions

One of the main objectives of this project was not simply to reproduce the screenshot, but to understand **why each CSS property was necessary**.

Some of the main decisions included:

* Using Flexbox for the card structure.
* Using `<picture>` for responsive image sources.
* Using `gap` to control the spacing between the cart icon and button text.
* Using `min-height: 100vh` to allow the page to occupy at least the full viewport height.
* Using CSS variables for repeated colors.
* Using a media query to switch from a horizontal to a vertical layout.
* Keeping the HTML semantic and letting CSS handle the visual presentation.

## 📂 Project structure

```text
.
├── images/
│   ├── favicon-32x32.png
│   ├── icon-cart.svg
│   ├── image-product-desktop.jpg
│   └── image-product-mobile.jpg
│
├── design/
│   ├── desktop-design.jpg
│   ├── mobile-design.jpg
│   └── active-states.jpg
│
├── index.html
├── style.css
└── README.md
```

## 🚀 Getting started

No build tool or dependency installation is required.

Clone the repository:

```bash
git clone <repository-url>
```

Open the project directory:

```bash
cd <project-directory>
```

Then open `index.html` in a browser.

## 🎨 Design

This project was built from the design provided by Frontend Mentor.

The objective was to reproduce:

* Desktop layout
* Mobile layout
* Typography
* Colors
* Spacing
* Border radius
* Product imagery
* Button hover state

## 🔗 Links

* [Frontend Mentor](https://www.frontendmentor.io/)
* [My GitHub](https://github.com/alexandre-delsol)
* [My Frontend Mentor profile](https://www.frontendmentor.io/profile/alexandre-delsol)

## 👤 Author

**Alexandre DELSOL**

Frontend / Full-Stack Developer in training, currently strengthening my frontend fundamentals through practical projects and Frontend Mentor challenges.

