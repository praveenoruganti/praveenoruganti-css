# CSS Animations

**Why CSS Animations?**
- Makes animating web elements much easier
- Eliminates the need for JavaScript/JQuery for a lot of animation effects
- Super easy once you get the hang of it

Lets see the below properties
- @keyframes
- animation-name
- animation-duration
- animation-delay
- animation-iteration-count
- animation-direction
- animation-timing-function
- animation-fill-mode
- animation


**What are CSS Animations?**
An animation lets an element gradually change from one style to another.You can change as many CSS properties you want, as many times you want.To use CSS animation, you must first specify some keyframes for the animation.Keyframes hold what styles the element will have at certain times.

**@keyframes**
When you specify CSS styles inside the @keyframes rule, the animation will gradually change from the current style to the new style at certain times.
To get an animation to work, you must bind the animation to an element.


**HTML**

```HTML
 <h1>CSS Animations</h1>
 <div class="animations"></div>
```

**CSS**

```CSS
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  margin: 25px;
}

.animations {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  /* animation-name: loop;
  animation-duration: 5s;
  animation-timing-function: linear;
  animation-delay: 2s;
  animation-iteration-count: infinite;
  animation-direction: alternate; */
  /* Shorthand animation property */
  animation: loop 5s linear 2s infinite alternate;
}

@keyframes loop {
  0% {
    background-color: red;
    left: 0px;
    top: 0px;
  }
  25% {
    background-color: yellow;
    left: 200px;
    top: 0px;
  }
  50% {
    background-color: blue;
    left: 200px;
    top: 200px;
  }
  75% {
    background-color: green;
    left: 0px;
    top: 200px;
  }
  100% {
    background-color: red;
    left: 0px;
    top: 0px;
  }
}

```

You can check out the [Demo](https://praveenoruganti.github.io/praveenoruganti-css/19_Animations/Demo).

You can also check out the Moving Car [Demo](https://praveenoruganti.github.io/praveenoruganti-css/19_Animations/Demo/Moving_Car.html).

### [Buy me a Coffee](http://bit.ly/2WryDT8)
