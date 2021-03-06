# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.jpeg)

### Links

- Solution URL: [Add solution URL here](https://github.com/adi71982/NFT-Preview-Card)
- Live Site URL: [Add live site URL here](https://adi71982.github.io/NFT-Preview-Card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- SCSS
- Mobile-first workflow


### What I learned

- Image Overlay
```css
.card-img  {
        
        position: relative;
        width: 100%;
        height: 300px;
        
        .nft-image {
            border-radius: 15px;
            transition: .5s ease;
            backface-visibility: hidden;
            width: 100%;
            height: 100%;
            opacity: 1;
        }

        .middle {
            transition: .5s ease;
            opacity: 0;
            position: absolute;
            width: 100%;
            height: 300px;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        &:hover {
            cursor: pointer;
            .nft-image {
                opacity: 0.3;
            }

            .middle {
                opacity: 1;
                background-color: rgba(0, 255, 247, 0.3);
            }
        }
    }
```
- Mobile first workflow
- Partial Scss


### Continued development

- Start to use partial scss and using body font size, giving relative font sizes to children.
- More modular css


### Useful resources

- [w3schools](https://www.w3schools.com/cssref/) - new to css, frequently need to see google.


## Author
- Frontend Mentor - [@adi71982](https://www.frontendmentor.io/profile/adi71982)
