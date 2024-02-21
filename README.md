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
<div class="card-grid__middle-cards">
        <div class="card-grid__card card-grid__second-card">
          <h3 class="card-grid__headings">Team Builder</h3>
          <p class="card-grid__paragraphs">Scans our talent network to create the optimal team for your project</p>
          <img class="card-grid__image" src="images/icon-team-builder.svg" alt="browser with home icon" />
        </div>

        <div class="card-grid__card card-grid__third-card">
          <h3 class="card-grid__headings">Karma</h3>
          <p class="card-grid__paragraphs">Regularly evaluates our talent to ensure quality</p>
          <img class="card-grid__image" src="images/icon-karma.svg" alt="lightbulb icon" />
        </div>
      </div>
```
<br>

The CSS in the media query for card grid is plain awesome!!

```css
:root {
    --space-60px: calc((60/16) * 1rem);
}

.main-content {
    margin: var(--space-60px) 0;
}

@media (min-width: 1200px){
    .card-grid {
        grid-template-areas:
            ".      second  ."
            "first  second  fourth"
            "first  third   fourth"
            ".      third   .";
    }
}
```

### Useful resources

Pro tip: use ALL resources!!

- [BEM naming style](https://css-tricks.com/bem-101/)
- [My gold standard practical CSS Grid reference](https://www.freecodecamp.org/news/learn-css-grid-by-building-5-layouts/) - I have been referring to this so many times over so many months because its that good!
- [Simple explanation on Grid template areas](https://www.w3schools.com/cssref/pr_grid-template-areas.php)
- [Learn to write good CSS by Kevin Powell](https://youtu.be/x4u1yp3Msao?si=8NcgyQzcAdNZ4UOx)

## Author

- GitHub - [Aldrin Sean Pereira](https://github.com/AldrinSeanPereira)
- Frontend Mentor - [@AldrinSeanPereira](https://www.frontendmentor.io/profile/yourusername)
- LinkedIn - [aldrinseanpereira](https://www.linkedin.com/in/aldrinseanpereira/)

## Acknowledgments

Thanks to frontend mentor and all the team in their discord server in the help section!!