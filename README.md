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
- [Acknowledgments](#acknowledgments)

## Overview

The overview is to build a QR code component and get it looking as close to the Figma design as possible

### Screenshot

![![QR code image](screenshots/Screenshot%202023-04-12%20at%2012.20.35.png)](./screenshot.jpg)

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

What I learned is that once the tutorials are finished and you sit in front of a blank VSC screen, it is as if everything learned has been forgotten! However, once I realised I must break the project down into bite sized chunks that made it easier to start. I began with the HTML and moved on to the CSS and used CSS grid to centre the component.

I learned the two methods of placing images within a component. One placing the image source within a conventional div element. The other using a picture element.

One aspect that is yet challenging me is inserting a media query in order to expand the the blue-grey background. The QR component does not alter in size on any screen.

Below is the aforementioned picture class. I eventually did not use it. The reason I used a conventional div element to contain the image was to be able to add border radius in the CSS, I had to add add overflow property with the value of hidden for the border radius to work.

- The HTML below is a picture element, which was new to me.

```html
<!-- the code below can be used instead of div
            <picture class="product-img">
            <source srcset="./images/image-qr-code.png" />
            <img src="./images/image-qr-code.png" alt="qr code image" />
          </picture>  
-->
```

- Below is the conventional div element containing image and source. The reason I used this code rather than picture element was the traditional div allowed the overflow: hidden property and value which allowed a border-radius.

```html
<div class="product-img">
  <img src="./images/image-qr-code.png" />
</div>
<div class="content"></div>
```

- The CSS code below is a class pointing to the image. Border radius would only work if overflow property was used with the hidden value.

```css
.product-img {
  width: 288px;
  height: 288px;
  margin: 1rem;
  border-radius: 1rem;
  overflow: hidden;
}
```

### Continued development

First and foremost I need to learn how to use media queries. I also need to focus on CSS Grid and Flexbox. Also, I need to learn the basics of Figma designs which give the exact details, such as font sizes and component sizes.

### Update ############ Update############### Update

The code has been updated thanks to both @ecemgo and @Panji200 at Frontend Mentor. Many thanks to them for their invaluable advice. They made it look so easy!

### Useful resources

Below are the resources I have used thus far.

- John Smilga has taught me HTML and CSS with his Udemy course. https://www.udemy.com/course/in-depth-html-css-course-build-responsive-websites/

- Coding Addict is John Smilga's excellent Youtube channel with many great frontend resources. https://www.youtube.com/@CodingAddict.

- Most of the Git and Github process I have learned from Colte Steele's excellent Udemy course https://www.udemy.com/course/git-and-github-bootcamp/.

## Author

- Frontend Mentor - [@John-Davidson-8](https://www.frontendmentor.io/profile/John-Davidson-8
