# Frontend Mentor - QR code component solution

This is a solution to the [Stats preview card component on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents


  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Built with](#Built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#Author)


### Screenshot

![Desktop](./Assets/Images/Screenshot%202024-11-16%20095705.png)
![Mobile](./images/Mobile.jpg)



### Links

- Solution URL: [Add solution URL here](https://www.frontendmentor.io/solutions/qr-code-component-solution-zOAC9qVUXY)
- Live Site URL: [Add live site URL here](https://hossein-np.github.io/)


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

The image and the demon have the same dimensions, and we defined a radius for the border, but it did not work well, so we finally defined the image display as a block.

```html
<main>
    <div class="card-box">
       <!-- Card image  -->
       <div class="card-box__img">
       </div>
        <!-- Card text content  -->
       <div class="card-box__text-content flex flex-col items-center">
        <h1 class="card-box__title interfont-preset-bold text-center">Get <mark>insights</mark> that help your business grow.</h1>
        <p class="card-box__caption text-center interfont-preset-regular">Discover the benefits of data analytics and make better decisions regarding revenue, customer experience, and overall efficiency.</p>
        <div class="card-box__numbers flex flex-col">
          <span class="text-center">10k+</span>
          <span class="text-center">314</span>
          <span class="text-center">12M+</span>
        </div>
       </div>
    </div>
   </main>
```
```css
.img {
  display: block;
}
```
```css
.card-box__numbers span {
  position: relative;
  animation: fadeIn 1s ease-in-out;
  font-size: 2.4rem;
}

.card-box__numbers span:nth-child(2) {
  margin: 2.4rem 0;
}

.card-box__numbers span::after {
  font-family: 'Lexend Deca';
  font-weight: normal;
  font-style: normal;
  font-size: 1.2rem;
  position: absolute;
  display: block;
  top: 3.2rem;
  left: 0;
  right: 0;
  text-align: center;
  color: #ffffff7a;
}

.card-box__numbers span:nth-child(1):after {
  content: "Companies";
}

.card-box__numbers span:nth-child(2):after {
  content: "Templates";
}

.card-box__numbers span:nth-child(3):after {
  content: "Queries";
}
```

### Useful resources

- [Tailwind css](https://tailwindcss.com/docs/installation) - use container and media query dimensions
- [CSS Reset](https://meyerweb.com/eric/tools/css/reset/) - css reset 



## Author

- Frontend Mentor - [@hossein-np](https://www.frontendmentor.io/profile/Hossein-NP)
- Github - [@hossein-np](https://github.com/Hossein-NP)

