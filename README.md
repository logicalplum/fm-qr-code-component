# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### Screenshot

![A card with QR code and invitation to Frontend Mentors centered on a light blue desktop screen](./screenshot.webp)

### Links

- Solution URL: [github.com/logicalplum/fm-qr-code-component](https://github.com/logicalplum/fm-qr-code-component)
- Live Site URL: [logicalplum.github.io/fm-qr-code-component](https://logicalplum.github.io/fm-qr-code-component/)

## My process

- Use vanilla HTML and CSS
- Self-host [Outfit Google Font](https://fonts.google.com/specimen/Outfit?preview.script=Latn), converting .ttl to .woff2 with Homebrew install of [Google's woff2](https://github.com/google/woff2)
- Link images, fonts, and css from `./assets/` folder
- Use design JPEG images to get approximate box padding and sizes
- Style to match visual look of design assets
- Check WCAG color contrast compliance with [CCA](https://vispero.com/lp/color-contrast-checker/)
- Convert png screenshot to webp format with [Google's webp converter](https://developers.google.com/speed/webp/)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

This challenge is my "Hello World" challenge on Frontend Mentor. Aside from the primary goal of learning how to build and submit a challenge, I was reminded of a few things I'd taken for granted working with CSS frameworks that normalize browser style differences.

- Browsers add a 8px margin to the `<body>` element to prevent unstyled HTML from pressing against the edges. I set `body { margin: 0; }` in CSS to allow body background to go to the edges.
- Default CSS box model (content-box) adds padding and border to box width and height, and that makes sizing _very_ tricky. Need to use `box-sizing: border-box;` in CSS to set box sizing independent of borders and padding. In had forgotten that `box-sizing` is not inherited, so setting that on the `body` element was not sufficient. It must be set on every sized element. I checked a popular normalizer, [modern-normalize](https://github.com/sindresorhus/modern-normalize), to find it set with a wild card.

Feedback from my initial submission identified more problems and opportunities for improvement:

- `index.html`: The page needs a level-1 heading. The "Improve your frontend skills..." line can do that; wrap in an `<h1>`.
- `style.css`: A `url()` reference should be relative to the css file rather than the root folder.
- `style.css`: Should set `width: 100%;` rather than `width: 100vw;` to get full width except for a scrollbar.
- `style.css`: Browser defaults for `<h1>` now needed to be taken into account.
- `README.md`: Fix a malformed URL that I had overlooked. (Didn't test.)

After the initial submission, I addressed the problems then accessed the Figma file to find typography and spacing details. As a _very_ occasional Figma user, it took a while to get reacquainted but found what I needed.

### Continued development

Current solution has only been tested in Chrome in macOS. Further testing in a variety of browsers and devices, including mobile devices, should be done to be confident of a robust solution.

### Useful resources

- [Self-hosting web fonts | Google Fonts](https://fonts.google.com/knowledge/using_type/self_hosting_web_fonts)
- [woff2 | GitHub](https://github.com/google/woff2)
- [woff2 | Homebrew Formulae](https://formulae.brew.sh/formula/woff2#default)
- [Colour Contrast Analyzer (CCA) | Vispero](https://vispero.com/lp/color-contrast-checker/)
- [WebP | Google for Developers](https://developers.google.com/speed/webp/)

## Author

- Website - [John F MacDonald](https://jfmacdonald.com)
- Frontend Mentor - [@logicalplum](https://www.frontendmentor.io/profile/logicalplum)
