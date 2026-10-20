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
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size (Desktop and Mobile responsive).
- See hover states for all interactive elements on the page.
- Receive an error message when the form is submitted if:
  - Any input field is empty. The message for this error says *"[Field Name] cannot be empty"*.
  - The email address is not formatted correctly. The message for this error says *"Looks like this is not an email"*.

### Screenshot

![](./screenshot.jpg)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)
## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- Vanilla JavaScript (Form Validation & DOM Manipulation)


### What I learned

During this project, I practiced and solidified several core web development concepts:
- Building responsive layouts using **CSS Grid** and **Flexbox**, switching smoothly from a two-column desktop layout to a single-column mobile layout.
- Implementing custom form validation with **JavaScript** to check empty fields and validate email formats.
- Dynamically toggling CSS classes (`classList.add` / `classList.remove`) to display error borders, background warning icons, and error text messages conditionally.

```html
<div class="field-group">
  <input type="text" placeholder="First Name" id="FirstName"/>
  <small class="error-text">First Name Cannot be empty</small>
</div>
```css
.field-group.error input {
  border: 2px solid hsl(0, 100%, 74%);
  background-image: url('images/icon-error.svg');
  background-repeat: no-repeat;
  background-position: right 15px center;
}
.field-group.error .error-text {
  display: block;
}
```Java
function checkInput(input) {
  let parent = input.parentElement;
  if (input.value.trim() === '') {
    parent.classList.add('error');
  } else {
    parent.classList.remove('error');
  }
}

## Author

- Website - [Rahaf](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

