# Frontend Mentor - Typemaster pre-launch landing page solution

This is a solution to the [Typemaster pre-launch landing page challenge on Frontend Mentor](). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - Typemaster pre-launch landing page solution](#frontend-mentor---typemaster-pre-launch-landing-page-solution)
  - [Table of contents](#table-of-contents)
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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./preview.jpg)


### Links

- Solution URL: [Add solution URL here](https://github.com/TayConn/typemaster_productSite)
- Live Site URL: [Add live site URL here](https://typemaster-product-site.vercel.app/)

## My process
- Rough out HTML semantics and start considering different sections of content
- start with mobile design first and roughing in the larger components then adding styling such as colors, fonts, positioning and flex-box directions.

### Built with

- Semantic HTML5 markup
- Sass preprocessor custom properties
- Flexbox
- Mobile-first workflow

### What I learned

Rather than using DIVs to swap out images based on the screensize, I used srcset and sizing within the image tags to grab the correct image to the screensize. 


```html
<img class="img-orange-kb orange-overlay" src="/assets/image-phone-and-keyboard-mobile.jpg" srcset="/assets/image-phone-and-keyboard-mobile.png 258w, /assets/image-phone-and-keyboard-tablet.jpg 428w, /assets/image-phone-and-keyboard-desktop.jpg 510w" sizes="(min-width: 60rem) 80vw, (min-width: 40rem) 90vw, 100vw" alt="A keyboard with an orange overlay next to a phone on a table">
```
-Using a filter over a provided image was new to me, usually I would just edit the image in a photoeditor and add an overlay there.
```css
.img-orange-kb{
            width: 8rem;
            height: 12rem;
            background-color: black;
            border-top-right-radius: 10px;
            border-bottom-right-radius: 10px;
            border-bottom-left-radius: 0;
            border-top-left-radius: 0;
            object-fit: cover;
            filter: invert(35%) sepia(60%) saturate(500%) hue-rotate(346deg) brightness(75%) contrast(125%);
        }
```


### Continued development

I'd really like to start using more image swapping methods via html into my workflow, its not always the best solution using a div with a class containing background images, especially for making the image accessible.


## Author

- Website - [Taylor Conn](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://tayconn.github.io/)
