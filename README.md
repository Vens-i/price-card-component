# Frontend Mentor - Pricing component with toggle solution

This is a solution to the [Pricing component with toggle challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/pricing-component-with-toggle-8vPwRMIC). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview and Challenge

This challenge is a pricing compenent that features 3 cards that display prices for a product. one card is features a gradient and slightly scaled up (not scaled on mobile screen) design that sets it apart from the others.

Additionally, there is a 'pill toggle' component that changes the price from the default monthly view into a yearly amount.

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- Control the toggle with both their mouse/trackpad and their keyboard (Click the toggle feature once or use tab to select, then use spacebar to move back and fort)

- **Bonus**: (Complete the challenge with just HTML and CSS)

Unfortunatly I needed JavaScript to add the change price feature.


### Screenshot

![](./images/wd-screenshot.png)


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- JavaScript

- [HTML5](https://developer.mozilla.org/en-US/docs/Web/HTML) - Markup
- [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) - for styles
- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) - for interactivity


### What I learned

This challenge relied heavily on CSS, I learned a great deal on dealing with CSS properties such as flex, padding, margins and scaling. Additionally, their was a strees on the importance of properly formatting my HMTL into divs and adding classes and IDs to be reffered to either in styling or in script files.

I also utilized multiple SVG files to create one background using CSS selector specificity to add a before and pseudo-elements like ::before and ::after.

I made use of JavaScript to interact with the DOM and add elements to my divs, which could then toggle a different CSS.

See below:

```html
        <input type="checkbox" name="toggle" id="toggle" onchange="toggleCheckbox()">
```
```css
.price-box .anually {
    display: none;
}

.show-anually .price-box .anually{
    display: block;
}

.show-anually .price-box .monthly{
    display: none;
}
```
```js
function toggleCheckbox() {
    var el = document.getElementById("flexy");
    el.classList.toggle("show-anually")
}
```

### Continued development

Currently I want to continue my developing my understanding of JavaScript as it is somewhat limited, while also familiarizing myself with CSS techniques that could make my Front-end journey much easier.


### Useful resources
- [MDN](https://developer.mozilla.org/en-US/) - For general understanding of the web technologies that I was using.

- [W3Schools](https://www.w3schools.com/howto/tryit.asp?filename=tryhow_js_toggle_class) - This helped me understand how to toggle between HTML classes using a JS function to then apply varying CSS.

- [Stack Overflow](https://stackoverflow.com/questions/3197702/html-checkbox-onclick-called-in-javascript) - This is a question that helped me understand how to get an 'onchange' attribute into my checkbox.


## Author

- Website - [Kervens Auguste] (Coming Soon)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)


## Acknowledgments

Major credit goes to Florin Pop, whose guides i used to complete this challenge. His guides can be found on his Youtube channel at -[https://www.youtube.com/@FlorinPop]

