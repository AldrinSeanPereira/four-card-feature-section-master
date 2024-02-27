# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![four-card-feature-section-master screenshot](images/four-card-feature-section-master.png)

### Links

- Solution URL: [Link](https://github.com/AldrinSeanPereira/four-card-feature-section-master)
- Live Site URL: [Link](https://iridescent-dieffenbachia-9ce774.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- BEM naming convention
- CSS Grid
- Mobile-first workflow

### What I learned

This is my first project using CSS Grid throughout. 

It also showcases my ability to create high quality maintainable code using BEM naming convention and custom reusable properties in CSS 

Combining the BEM naming + Custom properties + CSS Grid made me feel so happy to make this project

```html
<div class="card-grid__card card-grid__card--cyan">
  <h3 class="card-grid__headings">Supervisor</h3>
  <p class="card-grid__paragraphs">Monitors activity to identify project roadblocks</p>
  <img class="card-grid__image" src="images/icon-supervisor.svg" alt="magnifying glass icon" />
</div>
```
<br>

The CSS in the media query for card grid is plain awesome!!

```css
:root {
    --space-10px: calc((10/16) * 1rem);
}

.card-grid__card--cyan {
    background-image: linear-gradient(
        var(--color-Cyan) 2%,
        transparent 2%
    );
}

@media (min-width: 1200px){
    .card-grid {
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: repeat(4, 1fr);
    }

    .card-grid__card:nth-of-type(1) {
        grid-column: 1;
        grid-row: 2 / span 2;
    }

    .card-grid__card:nth-of-type(2) {
        grid-column: 2;
        grid-row: 1 / span 2;
    }

    .card-grid__card:nth-of-type(3) {
        grid-column: 2;
        grid-row: 3 / span 2;
    }

    .card-grid__card:nth-of-type(4) {
        grid-column: 3;
        grid-row: 2 / span 2;
    }
}
```

### Useful resources

Pro tip: use ALL resources!!

- [BEM naming style](https://css-tricks.com/bem-101/)

- CSS Grid study references:
  - start here with [Grid Garden](https://cssgridgarden.com/)
  - Article 1 : [CSS Grid theory - simple version to build more knowledge](https://www.freecodecamp.org/news/css-grid-tutorial-with-cheatsheet/)
  - Article 2 : [How to use CSS Grid practically ](https://www.freecodecamp.org/news/learn-css-grid-by-building-5-layouts/) - I have been referring to this so many times over so many months because its that good!
  - Article 3 : [CSS Grid theory - long version for reference](https://www.freecodecamp.org/news/complete-guide-to-css-grid/)
- [Learn to write good CSS by Kevin Powell](https://youtu.be/x4u1yp3Msao?si=8NcgyQzcAdNZ4UOx)

## Author

- GitHub - [Aldrin Sean Pereira](https://github.com/AldrinSeanPereira)
- Frontend Mentor - [@AldrinSeanPereira](https://www.frontendmentor.io/profile/yourusername)
- LinkedIn - [aldrinseanpereira](https://www.linkedin.com/in/aldrinseanpereira/)

## Acknowledgments

Thanks to frontend mentor and all the team in their discord server in the help section!!