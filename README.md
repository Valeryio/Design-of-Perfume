# Frontend Mentor - Product preview card component

![Design preview for the Product preview card component coding challenge](/ressources/images/solution.jpg)

## Welcome! 👋

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa).

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Links

- Solution URL: [Add solution URL here](https://design-of-perfume.vercel.app/)
- Live Site URL: [Add live site URL here](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa)


## My process

This is an update. I just read a tons of articles, and learn about HTML semantics, and follow some youtube tutorials to learn from some very great developers. I put the link in the ressources !


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

I learned a bunch of stuffs. Started with a great way to structure its CSS project.
- Using normalise CSS files ([Use this one of Josh Comeau](https://www.joshwcomeau.com/css/custom-css-reset/))

- Creating not-only **color variables**, but also fonts...
```css
:root
{
    /*
    // Font accentuated and base font used through the project    */

    --ff-accent: 'Fraunces', serif;
    --ff-base: 'Montserrat', sans-serif;

    --fw-bold: 700;
    --fw-regular: 500;
}

```

- Using local scope of variables in CSS
```css
.product
{
    /*Local variables*/
    --content-padding: 1.5rem;
    --content-spacing: 0.5rem;

    display: grid;
    overflow: hidden;
    max-width: 600px;
    min-width: 360px;
    border-radius: 0.5rem;
    transition: box-shadow ease-in-out 0.5s;
    background-color: var(--clr-neutral-white);
}

```

- A great way to design buttons in CSS
```css
.button:is(:hover, :focus)
{
    background-color: var(--clr-primary-dark-cyan);
    
}

.button[data-icon="shopping-cart"]::before
{
    content: '';
    width: 15px;
    height: 16px;
    background-image: url(/ressources/icons/icon-cart.svg);
}
```

- A new way to help screen-reader that increase accessibility
```css
.visually-hidden:not(:focus):not(:active)
{
    clip: rect(0 0 0 0);
    clip-path: inset(50%);
    height: 1px;
    overflow: hidden;
    position: absolute;
    white-space: nowrap;
    width: 1px;
  }

```



### Continued development

Yeah, I have to more invest in layout designing with modern
CSS tools like grid and flex. Just focus on it for the future days! 🚀🚀🚀

### Useful resources

- [Kevin Powell Youtube video on it!](https://youtu.be/B2WL6KkqhLQ)

