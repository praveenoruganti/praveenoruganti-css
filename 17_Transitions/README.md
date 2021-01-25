


# CSS Transitions



 CSS transitions allows you to change property values smoothly, over a given duration.
- transition
- transition-delay
- transition-duration
- transition-property
- transition-timing-function

To create a transition effect, you must specify two things
- the CSS property you want to add an effect to
- the duration of the effect
**Note**: If the duration part is not specified, the transition will have no effect, because the default value is 0.

The transition-timing-function property specifies the speed curve of the transition effect.

The transition-timing-function property can have the following values:
- ease - specifies a transition effect with a slow start, then fast, then end slowly (this is default)
- linear - specifies a transition effect with the same speed from start to end
- ease-in - specifies a transition effect with a slow start
- ease-out - specifies a transition effect with a slow end
- ease-in-out - specifies a transition effect with a slow start and end
- cubic-bezier(n,n,n,n) - lets you define your own values in a cubic-bezier function

The transition-delay property specifies a delay (in seconds) for the transition effect.

**HTML**

```HTML
<h1>The transition Property</h1>
<p>Hover over the div element below, to see the transition effect.</p>
<h1>The transition effect will start when the specified CSS property (width) changes value.</h1>
<div class="transition1"></div>
<br>

<h1>Transition effect for both the width and height property</h1>
<div class="transition2"></div>
<br>

<h1>The transition-timing-function Property</h1>
<p>Hover over the div elements below, to see the different speed curves:</p>
<br>
<div class="transition-timing-function transition-timing-function-linear">linear</div><br>
<div class="transition-timing-function transition-timing-function-ease">ease</div><br>
<div class="transition-timing-function transition-timing-function-ease-in">ease-in</div><br>
<div class="transition-timing-function transition-timing-function-ease-out">ease-out</div><br>
<div class="transition-timing-function transition-timing-function-ease-in-out">ease-in-out</div><br>

<h1>The transition-delay Property</h1>
<p>Hover over the div element below, to see the transition effect:</p>
<br>
<div class="delay"></div>
<br>

<h1>Transition + Transform</h1>
<p>Hover over the div element below:</p>
<br>
<div class="trans"></div>
<br>

<h1>Using The transition Shorthand Property</h1>
<p>Hover over the div element below, to see the transition effect:</p>
<br>
<div class="transShort"></div>
<br>

<h1>Hover Me</h1>
<div class="circle">Hover Me</div>

```

**CSS**

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

div {
    margin: 25px;
}

.transition1 {
    width: 100px;
    height: 100px;
    background: red;
    transition: width 2s;
}

.transition1:hover {
    width: 300px;
}

.transition2 {
    width: 100px;
    height: 100px;
    background: red;
    transition: width 2s, height 4s;
}

.transition2:hover {
    width: 300px;
    height: 300px;
}

.transition-timing-function {
    width: 100px;
    height: 100px;
    background: red;
    transition: width 2s;
}

.transition-timing-function-linear {
    transition-timing-function: linear;
}

.transition-timing-function-ease {
    transition-timing-function: ease;
}

.transition-timing-function-ease-in {
    transition-timing-function: ease-in;
}

.transition-timing-function-ease-out {
    transition-timing-function: ease-out;
}

.transition-timing-function-ease-in-out {
    transition-timing-function: ease-in-out;
}

.transition-timing-function:hover {
    width: 300px;
}

.delay {
    width: 100px;
    height: 100px;
    background: red;
    transition: width 3s;
    transition-delay: 1s;
}

.delay:hover {
    width: 300px;
}

.trans {
    width: 100px;
    height: 100px;
    background: red;
    transition: width 2s, height 2s, transform 2s;
}

.trans:hover {
    width: 300px;
    height: 300px;
    transform: rotate(180deg);
}

.transShort {
    width: 100px;
    height: 100px;
    background: red;
    transition: width 2s linear 1s;
}

.transShort:hover {
    width: 300px;
}

.circle {
    width: 100px;
    padding: 50px 0;
    line-height: 0;
    background: linear-gradient(45deg, black, darkred);
    color: white;
    border-radius: 50px;
    cursor: pointer;
    text-align: center;
    transition: 1s ease;
}

.circle:hover {
    background: linear-gradient(45deg, black, limegreen);
    transform: rotate(360deg);
}
```

You can check out the [Demo](https://praveenorugantitech.github.io/praveenorugantitech-css-course/18_Transitions/Demo){:target="_blank"}.




