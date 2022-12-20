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
- [Author](#author)

## Overview
 I really enjoyed this challenge and writing the documentation for it. This is my first time writing fully documentation on the building process and I look forward to doing it more with every new project I take on. Enjoy :D!  
### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

- When starting a Front-End Mentor Project I usually spend some time analyzing the layout and brainstorming the best way to handle certain parts of the project. for this one in particular i new it would be a bit challenge because i havent coded in almost 3 months so I made sure to take my time on this step.

- My next step is to dive into the files and build out my html. while doing this I usually have the mobile design pulled up on another screen and I make sure to get the HTML as close to the finish product as possilble before moving on to CSS.

- My last step is to begin my CSS, durring the beginning of any project I reset my css and look for common colors and typography to use as custom css properties. Moving forward I keep a small window of the html open to carfully style each element/div from top to bottom. this insures that the page will load seamlessly. I also make sure to carfully follow the design one step at a time. If i get very excited about something or have a sudden idea for the stying of a certain componet i allow my self to jump forward to it but during the end of the project I go through everything to makes sure all elements are sytled in the order the are written in in my HTML ( from top to bottom).

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I gained and revised so much knowledge by doing this project but I beileved the thing Istruggled with the most was overthinking it. The follow paragraphs serve as an example of how I was truly overthinking alot of the building process.

     One of my best examples of over thinking was when I started focusing on the hero image and its hover state. In my mind I wanted to create a div that I would later set the background image for with css and nested in that div would be another div containing the svg. My original thoughts were to set the display to none on the nested div and then use the hover pseudo-class to make it reappear.. I thought I could use diplay block for this lol. Here is what that original code looked like as well a screenshot of the outcome:

```html
<div class="hero-image">
  <div class=hero-hover>
    <svg></svg>
  </div>
</div>
```

```css
.hero-image {
  background-image: url(images/image);
  etc.
}
.hero-hover{
  display: none;
  background-color: hsla(178, 100%, 50%,);
}
.hero-hover:hover{
  display: block;
  ect.
}
```
![](.images/Screenshot%202022-12-20%20at%203.15.23%20PM.png)

      I realized using display none was not working and decided to try using opacity instead. It was perfect I set hover to opacity of 0 and and used the hover puesdo class to set its opacity to 1. here is what that looked like as well a screenshot of the outcome:

```html
<div class="hero-image">
  <div class=hero-hover>
    <svg></svg>
  </div>
</div>
```

```css
.hero-image {
  background-image: url(images/image)
  etc.
}
.hero-hover{
  opacity: 0;
  background-color: hsla(178, 100%, 50%,);
  etc.
}
.hero-hover:hover{
  opacity: 1;
  tranistion: 0.3s
  etc.
}
```
![](.images/Screenshot-2.png)

      This would have been perfect but I hit another road block. When I put the entire div to an opacity of 1 the backgroud color of the div was also an opacity of 1. It took me a long time to figure out how I could get the svg to an opacity of 1 while making the opacity of the BG-color more like  .50 % and finally it dawned on me. I had been overthinking the entire thing. My reslolution was to change the background color it self by adding an opacity of .5 to it. I FIXED IT :D Here is what the code looked like as well a screenshot of the outcome:

```html
<div class="hero-image">
  <div class=hero-hover>
    <svg></svg>
  </div>
</div>
```

```css
.hero-image {
  background-image: url(images/image)
  etc.
}
.hero-hover{
  opacity: 0;
  background-color: hsla(178, 100%, 50%, 0.534);
  etc.
}
.hero-hover:hover{
  opacity: 1;
  tranistion: 0.3s
  etc.
}
```
![](.images/Screenshot-3.png)

### Continued development

In resolution I learned that overthinking can be the obsticle that you are seraching for in your code. From this moment on I plan to lead my questions differently. Instead of thinking to myself "whats wrong with the code" or "why isnt this propert doing what its supposed to do", I will instead think out my own actions and figure out if i'm using the correct methods for the project at hand.

## Author

- Frontend Mentor - [@Hazel-Black](https://www.frontendmentor.io/profile/Hazel-Black)
- Youtube - [HazelBDev](https://www.youtube.com/channel/UCCDWcbyG8rf6TC41EDGD4Rg) more video's coming soon!!
