# CSS Float

CSS float is a property that forces any element to float (right, left, none, inherit) inside its parent body with the rest of the element to wrap around it. This property can be used to place an image or an element inside its container and other inline elements will wrap around it.

For eg. Images in newspaper and articles are placed in certain position with rest of the content wrapped around it.

One should keep in mind that this can only be applied to float the element horizontally (i.e. right or left ) not vertically.

float: left | right | none | inherit ;

- float:right;  /* Floats the element to right of it's container */
- float:left;   /*  Floats the element to left of it's container */
- float:none;   /*  It will restrict the element to float */
- float:initial;/*  The element remains to it's default position */
- float:inherit; /*  Enables the element to inherit the property from its parent element */

**HTML**

```HTML
<article>
    <h1>Images Floating in the Document Flow</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo sequi veniam ea
        enim nesciunt doloremque delectus sint consectetur qui magnam. Recusandae, hic quidem
        officia, asperiores sit libero sapiente totam eum.</p>
    <figure class="l left"><img src="PraveenOruganti.jpg" alt="Praveen Oruganti">
        <figcaption>Floating Left</figcaption>
    </figure>
    <p>Doloribus nisi ratione necessitatibus unde veritatis commodi veniam quas eaque fugiat
        nihil esse, id? Tempora quis quod impedit quia, facere incidunt, voluptatum dicta
        in dolores suscipit temporibus quam eos odit?</p>
    <figure class="r right"><img src="PraveenOruganti.jpg" alt="Praveen Oruganti">
        <figcaption>Floating Right</figcaption>
    </figure>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo sequi veniam ea
        enim nesciunt doloremque delectus sint consectetur qui magnam. Recusandae, hic quidem
        officia, asperiores sit libero sapiente totam eum.</p>
    <p>Doloribus nisi ratione necessitatibus unde veritatis commodi veniam quas eaque fugiat
        nihil esse, id? Tempora quis quod impedit quia, facere incidunt, voluptatum dicta
        in dolores suscipit temporibus quam eos odit?</p>
</article>
```

**CSS**

```CSS
.left {
  float: left;
  margin-right: 1em;
}

.right {
  float: right;
  margin-left: 1em;
}

img {
  width: 300px;
  height: 200px;
}

* {
  box-sizing: border-box;
}

body {
  background-color: #1d1f1f;
}

article {
  background-color: white;
  padding: 1em;
  width: 65%;
  margin: 0 auto;
  border: 5px solid #e18728;
}

h1 {
  text-align: center;
}

p {
  font-family: sans-serif;
}

figure {
  text-align: center;
  text-transform: uppercase;
  padding: 0.2em;
  margin: 0;
}

figure img {
  max-width: 100%;
}

@media all and (max-width: 1100px) {
  article {
    width: 80%;
  }
}

@media all and (max-width: 950px) {
  article {
    width: 95%;
  }
}

```

You can check out the [Demo](https://praveenorugantitech.github.io/praveenorugantitech-css/11_Float/Demo){:target="_blank"}.




