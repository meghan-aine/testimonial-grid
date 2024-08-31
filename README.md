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



## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

**Desktop:**

![image](https://github.com/user-attachments/assets/be6bb502-a104-41df-b17a-e609875542a5)

**Mobile:**

<img width="317" alt="image" src="https://github.com/user-attachments/assets/14ce61d6-b4a2-4d45-8418-5d9cd35ab665">



### Links

- Solution URL: [https://github.com/meghan-aine/testimonial-grid](https://github.com/meghan-aine/testimonial-grid)
- Live Site URL: [https://meghan-aine.github.io/testimonial-grid/](https://meghan-aine.github.io/testimonial-grid/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

This was my first project using flexbox and grid. Flexbox is used within each testimonial, and grid is used to structure the testimonials. I used @media to stack the testimonials if the viewport is less than 550px.

Learning: everything that needs to be styled differently must be packaged into divs - and that turned out to be more than I had expected!

```html
      <!--Jonathan-->
      <div class="testimonial" id="jonathan">
        <div class = "flex-wrapper">
          <img src="./images/image-jonathan.jpg" alt="Image of Jonathan Walters" class="profile_pic"/>
          <div class="profile">
            <p class="name">Jonathan Walters</p>
            <p class="status">Verified Graduate</p>
          </div>  
        </div>  
        <p class="summary">The team was very supportive and kept me motivated</p>
        <p class="quote">“ I started as a total newbie with virtually no coding skills. I now work as a mobile engineer 
            for a big company. This was one of the best investments I’ve made in myself. ”</p>
      </div>
```
```css
@media screen and (max-width:550px) {
    #container {
        position: relative;
        top: 40px;
        display: grid;
        grid-template-columns: 1fr;
        grid-template-areas: "daniel"
        "jonathan"
        "jeanette"
        "patrick"
        "kira";
        gap: 2rem;
        margin: 10px 10px
}
```

