# Frontend Mentor - QR Code Component Solution

This is my solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid


### What I learned

**CSS Grid is the most concise way to center a single item in a full-page container.**

When you only need to center one element, Grid's `place-items` shorthand handles both axes in a single line. Flexbox can do the same job but requires two separate properties (`justify-content` + `align-items`). For a simple full-viewport wrapper like this, Grid wins on clarity.

```css
/* Grid approach — one line does both axes */
.page {
  min-height: 100vh;
  display: grid;
  place-items: center;
}

/* Flexbox equivalent — needs two lines */
.page {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
```

**CSS inheritance means you don't repeat yourself.**

Setting `font-family` once on `body` automatically passes it down to every child element — `h1`, `p`, everything inside `.card`. That's inheritance in action. You only override where you actually need something different.

```css
/* Set once on body... */
body {
  font-family: "Outfit", sans-serif;
}

/* ...and .card h1 and .card p automatically inherit it */
```

**Semantic HTML makes structure meaningful.**

Using `<main>` for the page wrapper and `<article>` for the card (instead of generic `<div>`s) communicates the purpose of each element to browsers and screen readers.

```html
<main class="page">
  <article class="card">
    ...
  </article>
</main>
```

### Continued development

- **CSS Flexbox & Grid** — I want to get more comfortable using both layout systems confidently, knowing when to reach for one over the other.
- **Responsive design** — I'd like to practice building layouts that adapt cleanly across different screen sizes using media queries.
- **CSS custom properties** — I started using variables but want to build a stronger habit of structuring them from the start of every project.
- **Semantic HTML** — I want to keep improving my instinct for choosing the right HTML elements to write more accessible and meaningful markup.

### Useful resources

- [Frontend Mentor](https://www.frontendmentor.io) - The platform that provided this challenge. Great for practicing real-world UI builds with a structured brief and design files.
- [MDN Web Docs - CSS Inheritance](https://developer.mozilla.org/en-US/docs/Web/CSS/Inheritance) - The go-to reference for understanding how CSS inheritance works. Helped me grasp which properties cascade down to child elements and which don't.

### AI Collaboration

- **Tool used:** GitHub Copilot
- **How I used it:** I had Copilot generate the full solution first, then reviewed the code carefully and rebuilt everything from scratch on my own.
- **What worked well:** This approach turned out to be a fast, practical way to learn — seeing the complete picture first gave me a clear target, and rewriting it myself locked in the concepts.
- **Key takeaway:** Going through this process gave me a solid understanding of CSS inheritance and how styles cascade and propagate through the DOM.


## Author

- Website - [Joseph Apelete Biossey](https://sites.google.com/view/josephbiossey/home?authuser=0)
- Frontend Mentor - [@joedrake0909](https://www.frontendmentor.io/profile/joedrake0909)
- Twitter - [@joedrake0909](https://x.com/joedrake0909)
