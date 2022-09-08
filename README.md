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

![](images/solution(dark).png)
![](images/solution(light).png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow
- media quary for dark mode
- keyframes animation (rotate, translate, skew and scale)


### What I learned

- How to use grid template area more effectively. Turns out that grid template row will affect the layout in grid template area, so i must amend both to get my desired result.
- How to apply "dark mode" to my website. It is the same as media quary for the width of the screen.
- How to use keyframes animation. Keyframes is like setting animation on the website with tools like rotate, skew, translate and skale on the time frame (0% till 100%).

To see how you can add code snippets, see below:

```css
/* keyframe animation example */
.boxGrid_boxCard:nth-child(4):hover{
  animation: spacewrap 1s 1;
}
@keyframes spacewrap{
  0%{
    transform: skew(0deg, 0deg);
  }
  25%{
    transform: skew(25deg, 0deg);
  }
  50%{
    transform: skew(0deg, 25deg);
  }
  100%{
    transform: skew(-5deg, -5deg);
  }
}

/* dark mode */
@media(prefers-color-scheme: dark){ 
body{
 background-color: black;
}
.boxGrid_boxCard{
background-color: black;
}
}
```

### Continued development

Would like to learn more on how to insert more animations in my website to make it more interactive to the users.

### Useful resources

- https://developer.mozilla.org/en-US/docs/Web/CSS/transform - Listing of some example on how to use rotate, skew, translate and scale
- https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes - This page helps on explaining how keyframes work
- https://www.w3schools.com/cssref/playdemo.asp?filename=playcss_box-shadow - this page reminds me on different things to tweaks on the shadow.
- https://www.youtube.com/watch?v=n3lcjY4Mm00 - This tutorial help me in inserting dark mode into the website.

## Author

- Frontend Mentor - [@Jetyun](https://www.frontendmentor.io/profile/Jetyun)
- Github - (https://github.com/Jetyun) 

## Acknowledgments

Thanks MDN tutorials for teaching how to use keyframes paired with rotate, skew, scale and translate. 
Thanks Kevin Powell for teaching how to implement dark mode in website.
Thanks Elaine Leung from Frontend Mentor for teaching on how to set media query more effectively.
