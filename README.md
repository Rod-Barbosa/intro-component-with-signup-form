# Frontend Mentor - Intro component with sign up form solution

This is a solution to the [Intro component with sign up form challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/intro-component-with-signup-form-5cf91bd49edda32581d28fd1). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
- See hover states for all interactive elements on the page
- Receive an error message when the `form` is submitted if:
  - Any `input` field is empty. The message for this error should say *"[Field Name] cannot be empty"*
  - The email address is not formatted correctly (i.e. a correct email address should have this structure: `name@host.tld`). The message for this error should say *"Looks like this is not an email"*

### Screenshot

![](./ScreenShotDesktop.png)
![](./ScreenShotDesktopNo.png)
![](./ScreenShotMobile.png)

### Links

- Solution URL: [Portfolio](https://gelatodigital.com/portfolio)
- Live Site URL: [rodrigos-intro-component-with-signup-form.netlify.app/](https://rodrigos-intro-component-with-signup-form.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- JavaScript

### What I learned

This exercise was all about details.
This is how I palced the "!" icon inside the input tag, without the need for position:absolute
```css
input:invalid {
    border: 1px solid red;
    background: url("./images/icon-error.svg") no-repeat 95% 50%;
    background-size: 1rem;
}
```
This is how to validae against empty input fields without the need for JS
```html
 <input type="text" placeholder="Last Name" required pattern=".*\S.*" id="lName">
```
This is how to make the correct error message disappear, without the need for JS
```css
#fName:valid~.noFName {
    display: none;
}
```

This is how to stop input field cliecked from becoming blue and breaking the color scheme of the website
```css
input:focus {
    outline: none !important;
    border: 1px solid black;
}
```

### Continued development

For sure JS is a usefull tool, but form validation is just a mess. I just hope I'll get better at it, at least with the submmit button, and information storage.

### Useful resources

- [regex for not empty input field](https://zellwk.com/blog/check-empty-input-css/)
- [error icon inside input field](https://www.digitalocean.com/community/tutorials/css-styling-form-input-validity)
- [form submit js](https://www.w3schools.com/howto/tryit.asp?filename=tryhow_js_validation_empty_input)
- [change input:focus border color](https://stackoverflow.com/questions/16156594/how-to-change-border-color-of-textarea-on-focus)

## Author

- Website - [Rodrigo Barbosa](https://www.gelatodigital.com)
- Frontend Mentor - [@Rod-Barbosa](https://www.frontendmentor.io/profile/Rod-Barbosa)

## Acknowledgments

Today is Valentine's day in my country, and I would like to thank all the women who let me alone today. Thank you. Little is more dangerous than a man who is without woman and happy about it.
