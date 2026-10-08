# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)
## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

#### Desktop
![](/assets/screenshots/desktop.png)

#### Tablet
![](/assets/screenshots/tablet.png)

### Mobile
![](/assets/screenshots/mobile.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties 
- Flexbox
- CSS Grid

### What I learned

I got a bit more exposure to clamp. I was happiest with how the clamp on the card's padding worked out. It's something I've used before but don't often reach for, and here it does the job without a bunch of extra media query rules. The anchors are predictable as the padding goes from 24px to 40px between a 375px and 432px viewport, which is exactly where the card itself changes size. 

I also learnt a bit more about how grid elements affect child component's sizing. For context, I reached for `max-width` on `.profile` without understanding the nuance of having `display: grid` on an element that wasn't `.profile`'s parent. The body was a grid item, and `margin: auto` was making it fit the size of its content. Because of that, `.profile` couldn't grow; it was effectively just fitting content. I moved the centering to the body so `.profile` became the grid item, and used `min()` to make the width sizing easier to manage.  

### Continued development

I was looking into cqi for the .profile container but my understanding was it only really applied to the child items and it didn't really seem like a good fit for this smaller project. Something to look into later.

The centering approach I ended up with, grid on the body and `width: min(384px, 100%)` on the card, isn't something I usually do, but I want to take it forward. I'm sure there are nuances I haven't hit yet, so I'll deal with the drawbacks project by project.

### Useful resources

- [PerfectPixel](https://www.welldonecode.com/perfectpixel/) - I used PerfectPixel to line up the Figma designs with the browser. Definitely helped with getting inconsistenties earlier and quickly. It's also free!

### AI Collaboration

- **Tool:** Claude Code.
- **How I used it:** to compare concepts and look at the downsides of approaches in the context of this project, mainly when I was stuck or at a standstill. I then checked what it said against MDN and CSS-Tricks. Most of the time I worked on my own and read docs. No code generation on this project.
- **What worked:** a quick sanity check, or a quick understanding of one approach against another for this specific project, before getting the fuller picture from vetted sources.
- **What didn't:** it sometimes brought up unrelated things. That was occasionally useful and often not relevant, so I took what I needed and ignored the rest.

## Author

- Frontend Mentor - [@nicholas-crawford](https://www.frontendmentor.io/profile/nicholas-crawford)
- Twitter - [@_nick_crawford_](https://www.twitter.com/_nick_crawford_)

