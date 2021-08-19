# Frontend Mentor - Fylo data storage component solution

This is a solution to the [Fylo data storage component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/fylo-data-storage-component-1dZPRbV5n). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow

### What I learned

In my last challenge, I struggled with moving elements around by pixels. It felt like a bandage solution and was messy as one thing would break everything else. Instead, I discovered using `vh` instead of `px`; it dramatically made things easier. 

I'm most proud of using `:after` on `div` elements to add a little bit more to it. This can be found on the tip of the `data-bar` and on desktop versions of the `remaining data`.

    #data-bar:after {
        content: '';
        background-color: white;
        border-style: solid;
        border-width: 1px;
        border-color: white;
        height: 11px;
        width: 11px;
        border-radius: 100%;
        position: absolute;
        margin-left: 43%;
        top: 1px;
    }

    .remaining-data:after{
        content: '';
        position: absolute;
        border-style: solid;
        border-width: 0px 23px 17px 0;
        border-color: transparent white;
        display: block;
        width: 0;
        z-index: 1;
        left: 15vh;
        top: 6.5vh;
    }

These are respectively the white circular tip of the data bar and the little triangle. It sure helped that I didn't have to create _another_ `div` element. 

### Continued development

If I were to continue developing this challenge, I would create more breakpoints for iPhones. I went for the bare minimum requirement of 375 and 1440.

### Useful resources

- [How to make a right triangle](https://stackoverflow.com/questions/45971545/how-can-i-make-an-speech-box-with-an-right-angle-triangle-css) - This helped me realize that using the `:after` tag was easier than creating a whole other `div`.

## Author

- Website - [GitHub](https://www.github.com/brandonnhem)
- Frontend Mentor - [@brandonnhem](https://www.frontendmentor.io/profile/brandonnhem)
