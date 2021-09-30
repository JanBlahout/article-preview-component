# Frontend Mentor - Article preview component solution

This is a solution to the [Article preview component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/article-preview-component-dYBN_pYFT). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See the social media share links when they click the share icon

### Links

- Live Site URL: https://thirsty-knuth-99402d.netlify.app/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Dekstop-first workflow
- Javascript

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<p class="link popup">
  <span class="popuptext" id="myPopup"></span>
</p>
```

```css
.popup {
  position: relative;
  display: inline-block;
  cursor: pointer;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/* The actual popup */
.popup .popuptext {
  visibility: hidden;
  display: flex;
  align-items: center;
  justify-content: space-around;
  width: 25rem;
  background-color: var(--dark-gray-blue);
  color: #fff;
  /* text-align: center; */
  border-radius: 6px;
  padding: 16px 32px;
  position: absolute;
  z-index: 1;
  bottom: 160%;
  left: 50%;
  margin-left: -125px;
  font-size: 1.4rem;
  font-family: 'Manrope', sans-serif;
  letter-spacing: 3px;
  color: var(--gray-blue);
}

/* Popup arrow */
.popup .popuptext::after {
  content: '';
  position: absolute;
  top: 100%;
  left: 50%;
  margin-left: -10px;
  border-width: 10px;
  border-style: solid;
  border-color: var(--dark-gray-blue) transparent transparent transparent;
}

/* Toggle this class - hide and show the popup */
.popup .show {
  visibility: visible;
  -webkit-animation: fadeIn 1s;
  animation: fadeIn 1s;
  z-index: 1;
}

/* Add animation (fade in the popup) */
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
```

```js
const proudOfThisFunc = () => {
  console.log('🎉');
};
```

### Continued development

I have to get better at CSS and positioning images / divs.

### Useful resources

https://www.w3schools.com/howto/tryit.asp?filename=tryhow_js_popup - This helped me for popup window.

## Author

- Frontend Mentor - https://www.frontendmentor.io/profile/JanBlahout
