# Frontend Mentor - Blog preview card solution

This is a solution to the Blog preview card challenge on Frontend Mentor(https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![](./assets/images/blogpreview_desktop.png)
![](./assets/images/blogpreview_mobile.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

Most of the concepts used in this project were not entirely new to me, but building the card helped me practise and reinforce them. The main new thing I learned was how to add custom fonts locally using @font-face.

During the build, I also:

Practised using positioning based on feedback from my previous QR Code challenge.
Continued improving my approach to responsive design by using relative sizing instead of relying solely on fixed pixel values.
Revisited the box-shadow property and became more comfortable recreating shadows from a design mock-up.
And how to reduce font size for smaller screens without using media queries.


```css
for addin already downloaded fonts from the folder
@font-face {
  font-family: 'Figtree';
  src: url('./assets/fonts/static/Figtree-ExtraBold.ttf') format('truetype');
  font-weight: 800;
  font-style: normal;
}

Using box-shadow to add the shadow
.cards {
  background-color: hsl(0, 0%, 100%);
  padding: 24px;
  border-radius: 20px;
  box-shadow: 10px 10px 5px 0 rgba(9, 0, 0, 0.75);
  max-width: 100%;
}

Using relative sizing instead of fixed value
.container {
  width: 90%;
  max-width: 384px;
  margin: 0 auto;
  padding: 96px 0;
  margin-bottom: 24px;
}

Using positon to syle my footer
.attribution {
  font-size: 0.6875rem;
  text-align: center;
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
}

example of how get the font-size to reduce based on screen size without media query
.description {
  font-size: clamp(0.875rem, 0.7857rem + 0.381vw, 1rem);
  font-weight: 500;
  color: hsl(0, 0%, 42%);
}

```


### Continued development

In future projects, I want to continue improving my responsive design skills by relying more on flexible sizing techniques rather than fixed dimensions. I also plan to become more comfortable working with custom fonts and recreating design details such as shadows and spacing with greater accuracy.

Additionally, I would like to further explore CSS positioning and layout techniques to build more polished and adaptable user interfaces across different screen sizes.

### Useful resources

- [Example resource 1](https://css-tricks.com/) - This helped me with everything flexbox. I really liked using it as it broke down everything concerning CSS.

- [Example resource 2](https://css-tricks.com/almanac/rules/f/font-face/) - This is an amazing article which helped me finally understand how to implement adding fonts from a downloaded/ included folder. I'd recommend it to anyone still learning this concept.

- [Example resource 3](https://stackoverflow.com/questions/35978790/bigger-fonts-on-smaller-screens-without-media-queries-or-javascript) - This is an amazing resource that helped me understand how I can to reduce font size for smaller screens without using media queries. And (https://clamp.font-size.app/) was the website i used to convert it.


## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)



## Acknowledgments

Thanks to Frontend Mentor for providing real-world frontend challenges that help developers improve their coding skills.
