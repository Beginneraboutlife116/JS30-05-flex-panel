# JS30-05-Flex panel
This is a solution to the [JS30-05-Flex Panels Image Gallery](https://courses.wesbos.com/account/access/62496c1ad3e09a449732a6f9/view/194130264).

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
- toggle the image gallery to appreciate the whole image by clicking.

### Screenshot
![desktop-inactive](./src/image/desktop-inactive.png)
![desktop-active](./src/image/desktop-active.png)
<div style="display: flex;">
  <img src="./src/image/mobile-inactive.png" width="50%" alt="mobile-inactive" />
  <img src="./src/image/mobile-active.png" width="50%" alt="mobile-active" />
</div>

### Links
- [Solution URL](https://github.com/Beginneraboutlife116/JS30-05-flex-panel)
- [Live Site URL](https://beginneraboutlife116.github.io/JS30-05-flex-panel/)

## My process

### Built with
- Semantic HTML5 markup
- CSS custom properties
- Flex box
- Mobile-first workflow

### What I learned
In this practice, I realized that it's a toggle events and also it's just a image gallery. So I decided to use CSS input checkbox to achieve that without JavaScript.

The most important things that I learned is 
1. `flex`: `flex` is a shorthand for `flex-grow`, `flex-basis`, `flex-shrink`. In the different viewport layout, they have different weight to impact themselves.
```css
.item { 
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
} 
/* default: flex: 0 1 auto; */
```
 - `flex-shrink` and `flex-basis` are optional.
   - `flex-grow`: defines the ability for a flex item to grow if necessary.
     - default: `1`
     - accepts a unit-less value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up.
   - `flex-shrink`: defines the ability for a flex item to shrink if necessary.
   - `flex-basis`: defines the default size of an element before the remaining space is distributed.
     - It has heavier weight than `width`.
   - [Sample](https://codepen.io/beginneraboutlife116/pen/RwQGvze)

### Continued development
I have found the font would have some latency when we load the page, so I will try to find the solution.
I have found the solution like `@font-face`.
Still try.

### Useful resources
- [The complete guid to Flex box](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This helped me for using `flex` property and knowing the basic of `flex`.
- [Making Google Fonts Faster in 2022](https://sia.codes/posts/making-google-fonts-faster/) - This is an amazing article which helped me finally understand how I can improve my google fonts loading, but I'm still testing. I'd recommend it to anyone want to improve the performance of loading fonts style.
- [How to host your own fonts made simple](https://www.youtube.com/watch?v=KzqQXDbDvus) - This is how Kevin using the `@font-face`, I still figure out which one is better? Self-hosting or Google Fonts link in HTML?

## Author
- [WeiKai](https://github.com/Beginneraboutlife116)