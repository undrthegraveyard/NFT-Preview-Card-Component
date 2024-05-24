## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

NFT Card Design Component

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./design/Final%20Design%20Desktop%20Preview.png)
![](./design/Final%20Design%20Tablet%20Preview.png)
![](./design/Final%20Design%20Mobile%20Preview.png)

### Links

- Solution URL:(https://github.com/undrthegraveyard/NFT-Preview-Card-Component.git)
- Live Site URL:(https://undrthegraveyard.github.io/NFT-Preview-Card-Component/)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

Using overlay to include hover state interaction in the hero image.

```html
<div class="nft__image-container">
      <img src="/images/image-equilibrium.jpg" alt="A 6-face cube standing on a flat surface" id="hero-image"/>
      <div class="nft__overlay">
        <img src="./images/icon-view.svg" alt="View icon" class="view-icon"/>
      </div>
    </div>
```
```css
.nft__overlay{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: hsla(178, 100%, 50%, 0);
    display: flex;
    justify-content: center;
    align-items: center;
    transition: 0.3s ease-in-out;
}
.view-icon {
    opacity: 0;
}
/* Hover Interation */
.nft__overlay:hover, .nft__overlay:focus {
    background-color: hsla(178, 100%, 50%, 0.5);
    .view-icon {
        opacity: 1;
    }
}
```
## Author

- Website - [Shivam Agarwal](https://www.shivamagarwal.au)
- Frontend Mentor - [@undrthegraveyard](https://www.frontendmentor.io/profile/undrthegraveyard)
- Twitter - [@shivam_agarwaal](https://twitter.com/shivam_agarwaal)