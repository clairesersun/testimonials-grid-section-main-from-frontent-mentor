# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![Desktop Design](/images/desktop.png)
![Mobile Design](/images/375%20-%201.png)
![Mobile Design](/images/375%20-%202.png)

### Links

- Solution URL: [https://github.com/clairesersun/testimonials-grid-section-main-from-frontent-mentor](https://github.com/clairesersun/testimonials-grid-section-main-from-frontent-mentor)
- Live Site URL: [https://clairesersun.github.io/testimonials-grid-section-main-from-frontent-mentor/](https://clairesersun.github.io/testimonials-grid-section-main-from-frontent-mentor/)

## My process

- Created a repository and copied challenge files
- Created HTML Structure
- Built initial CSS Styling
- Utilized a live port and Chrome's inspect tool to style mobile screen-size
- Switched view to desktop and created a media query to style the grid layout
- Checked for inconsistencies and errors

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

I learned how to use grids and how to implement them with a mobile-first mindset.

I implemented the grid layout in a media query so that I could build up from a screen-size of 375px:

```css
@media (min-width: 376px) {
  .wrapper {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-auto-rows: minmax(100px, auto);
    padding: 10%;
  }
  .one {
    grid-column: 1 / span 2;
    grid-row: 1;
    background: hsl(263, 55%, 52%) url("images/bg-pattern-quotation.svg") right 20%
      top;
    background-repeat: no-repeat;
    background-size: 18%;
  }

  .two {
    grid-column: 3;
    grid-row: 1;
  }
  .three {
    grid-column: 4;
    grid-row: 1 / span 2;
  }
  .four {
    grid-column: span 1;
    grid-row: 2;
  }
  .five {
    grid-column: span 2;
    grid-row: 2 / span 1;
  }
}
```

## Author

- Website - [Claire Sersun](https://www.clairesersun.com/)
- Frontend Mentor - [@clairesersun](https://www.frontendmentor.io/profile/clairesersun)
- LinkedIn - [Claire Sersun](https://www.linkedin.com/in/clairesersun/)
