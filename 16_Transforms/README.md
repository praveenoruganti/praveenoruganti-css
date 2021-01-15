


# CSS Transforms

![screenshot of the app](https://raw.githubusercontent.com/praveenorugantitech/praveenorugantitech-express-js/master/tech.PNG)

 CSS transforms allow you to move, rotate, scale, and skew elements.

**Possible values are**
- translateX()
- translateY()
- translate()
- scaleX()
- scaleY()
- scale()
- skewX()
- skewY()
- skew()
- matrix()
- rotateX()
- rotateY()
- rotateZ()
- rotate()

**translate()**
The translate() method moves an element from its current position (according to the parameters given for the X-axis and the Y-axis).

**rotate()**
The rotate() method rotates an element clockwise or counter-clockwise according to a given degree.
Using positive values it will rotate clockwise and via negative values it will rotate the element counter-clockwise.

**scale()**
The scale() method increases or decreases the size of an element (according to the parameters given for the width and height).

**skew()**
The skew() method skews an element along the X and Y-axis by the given angles.

**matrix()**
The matrix() method combines all the 2D transform methods into one.
The matrix() method take six parameters, containing mathematic functions, which allows you to rotate, scale, move (translate), and skew elements.
The parameters are as follow: matrix(scaleX(),skewY(),skewX(),scaleY(),translateX(),translateY())

**rotateX()**
The rotateX() method rotates an element around its X-axis at a given degree

**rotateY()**
The rotateY() method rotates an element around its Y-axis at a given degree

**rotateZ()**
The rotateZ() method rotates an element around its Z-axis at a given degree


**HTML**

```HTML
<h1>The translate() Method</h1>
<p>The translate() method moves an element from its current position.</p>
<div class="translate">
    This div element is moved 50 pixels to the right, and 100 pixels down from its current position.
</div>

<br><br><br><br><br><br><br><br>

<h1>The rotate() Method</h1>
<p>The rotate() method rotates an element clockwise or counter-clockwise.</p>
<br><br>
<div>
    This a normal div element.
</div>

<div class="rotateClock">
    This div element is rotated clockwise 20 degrees.
</div>

<div class="rotateCounterClock">
    This div element is rotated counter clockwise 20 degrees.
</div>

<br><br><br><br>

<h1>The scale() Method</h1>
<p>The scale() method increases or decreases the size of an element.</p>

<br>

<div class="scaleIncrease">
    This div element is two times of its original width, and three times of its original height.
</div>

<div class="scaleDecrease">
    This div element is decreased to be half of its original width and height.
</div>

<h1>The skew() Method</h1>
<p>The skew() method skews an element into a given angle.</p>
<br>
<div>
    This a normal div element.
</div>

<div class="skew">
    This div element is skewed 20 degrees along the X-axis, and 10 degrees along the Y-axis.
</div>

<br>

<h1>The matrix() Method</h1>
<p>The matrix() method combines all the 2D transform methods into one.</p>
<br>

<div>
    This a normal div element.
</div>

<div class="matrix1">
    Using the matrix() method.
</div>

<div class="matrix2">
    Another use of the matrix() method.
</div>

<br>

<h1>The rotateX() Method</h1>
<p>The rotateX() method rotates an element around its X-axis at a given degree.</p>
<br>
<div>
    This a normal div element.
</div>

<div class="rotateX">
    This div element is rotated 150 degrees.
</div>

<br>
<h1>The rotateY() Method</h1>
<p>The rotateY() method rotates an element around its Y-axis at a given degree.</p>
<br>
<div>
    This a normal div element.
</div>

<div class="rotateY">
    This div element is rotated 150 degrees.
</div>

<br>

<h1>The rotateZ() Method</h1>
<p>The rotateZ() method rotates an element around its Z-axis at a given degree.</p>
<br>
<div>
    This a normal div element.
</div>

<div class="rotateZ">
    This div element is rotated 90 degrees.
</div>

```

**CSS**

```CSS
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

div {
    width: 300px;
    height: 100px;
    background: linear-gradient(45deg, black, darkred);
    border: 1px solid black;
    color: white;
}

.translate {
    transform: translate(50px, 100px);
}

.rotateClock {
    transform: rotate(20deg);
}

.rotateCounterClock {
    transform: rotate(-20deg);
}

.scaleIncrease {
    margin: 150px;
    transform: scale(2, 3);
}

.scaleDecrease {
    margin: 150px;
    transform: scale(0.5, 0.5);
}

.skew {
    transform: skew(20deg, 10deg);
}

.matrix1 {
    transform: matrix(1, -0.3, 0, 1, 0, 0);
}

.matrix2 {
    transform: matrix(1, 0, 0.5, 1, 150, 0);
}

.rotateX {
    transform: rotateX(150deg);
}

.rotateY {
    transform: rotateY(150deg);
}

.rotateZ {
    transform: rotateZ(90deg);
}
```

You can check out the [Demo](https://praveenorugantitech.github.io/praveenorugantitech-css/17_Transforms/Demo){:target="_blank"}.



