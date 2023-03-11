# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./images/Final%20project.png)

### Links

- Solution URL: [Huddle page](isaacvf-dev.github.io)
- 

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I got to use some icons from font-awesome. I learned a lot styling that, especially using some pseudo elements like ::after, :nth-child(). In addition, I remembered some concepts about box-shadow and transition.

I see that I should study more responsive web design. Most of my struggles while doing this project where related to the responsiveness of the page.


```html
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css" integrity="sha512-SzlrxWUlpfuzQ+pcUCosxcglQRNAq/DZjVsC0lE40xsADsfeQoEypE+enwcOiGjk/bSuGGKHEyjSoQ1zVisanQ==" crossorigin="anonymous" referrerpolicy="no-referrer" />

  <div class="social">
    <a href="#">
      <i class="fab fa-facebook-f"></i>
    </a>
    <a href="#">
      <i class="fab fa-twitter"></i>
    </a>
    <a href="#">
      <i class="fab fa-instagram"></i>
    </a>
  </div>
  
  <a href="#" >Register</a>
```
```css
.social a i::after {
  content: '';
  position: absolute;
  height: 40px;
  width: 40px;
  border: 2px solid #fff;
  border-radius: 50%;
  left: -15px;
  bottom: -13px;
  transition: all .3s ease;
}

.information a {
  display: inline-block;
  text-decoration: none;
  font-family: 'Poppins', sans-serif;
  background-color: #fff;
  padding: 13px 50px;
  border-radius: 25px;
  box-shadow: 0 8px 17px -8px rgba(0, 0, 0, 0.8);
  transition: all .3s ease;
}

@media only screen and (max-width: 768px) {
  .main {
    flex-direction: column;
    text-align: center;
  }

  .information h1 {
    font-size: 26px;
  }

  .social {
    text-align: center;
    margin-top: 50px;
  }

  .information a {
    padding: 10px 70x;
  }

  footer {   
    margin-top: 40vh;       
  }
}

.social a i:hover::after {
  border-color: hsl(300, 69%, 71%);
}
```
### Continued development

I see that I should study more responsive web design. Most of my struggles while doing this project where related to the responsiveness of the page.


### Useful resources

- [:hover::after](https://stackoverflow.com/questions/13233991/combine-after-with-hover) - This helped me understand the use of :hover::after.
- [Pseudo-elements](https://www.w3schools.com/css/css_pseudo_elements.asp) - This is an amazing article which helped me remember the use of pseudo-elements. I'd recommend it to anyone still learning this concept.

## Author

- Frontend Mentor - [@Isaacvf-dev](https://www.frontendmentor.io/profile/Isaacvf-dev)
- LinkedIn - [Isaac Vieira](https://www.linkedin.com/in/isaac-vieira-francelino/)


