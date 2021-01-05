# CSS Background

Here with the CSS background properties.

- **opacity**  property specifies the opacity/transparency of an element. It can take a value from 0.0 - 1.0. The lower value, the more transparent.
- **background-color**  Defines an element's background color.
- **background-image**  Defines an element's background image. i.e.. url("")
- **repeat**  Specify whether/how the background image is tiled. i.e.. no-repeat,repeat-x,repeat-y
- **background-attachment**  Specify whether the background image is fixed in the viewport or scrolls. i.e.. scroll, fixed
- **background-position**  Defines the origin of a background image. i.e.. top,left,right,bottom,center
- **background-size**  Specifies the size of the background images.
- **Shorthand Property background** color image repeat attachment position;

**HTML**

```HTML
<h2>Background Color</h2>
<div class="bg-color">
    <h1> I am with Teal Color Background</h1>
</div>
<h2>Background Image</h2>
<div class="bg-image">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
        magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat
        nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit
        anim id est laborum.</p>
</div>
<h2>Background Attachment- fixed</h2>
<div class="bg-attachment">

</div>
<h2>Background Repeat - no-repeat</h2>
<div class="bg-repeat">

</div>

<h2>Background Position - bottom right</h2>
<div class="bg-position">

</div>
<h2>Background Size - Cover</h2>
<div class="bg-size">

</div>
<h2>Gradient</h2>
<div class="gradient">
</div>

```

```CSS
h1 {
  opacity: 0.2;
}


body {
  font-family: Arial, Helvetica, sans-serif;
}

.bg-color {
  background-color: teal;
}

.bg-image {
  padding: 15px;
  width: 500px;
  box-shadow: 0 0 10px black;
  background-image: url("img/image2.jpg");
}

.bg-repeat {
  width: 500px;
  height: 300px;
  box-shadow: 0 0 10px black;
  /* background-color: lightsalmon;
  background-image: url("img/image4.jpg");
  background-repeat: no-repeat;
  background-position: top right;
  background-attachment: scroll; */
  background: lightsalmon url("img/image4.jpg") no-repeat scroll top right;
}

.bg-position {
  width: 500px;
  height: 300px;
  box-shadow: 0 0 10px black;
  background: lightsalmon url("img/image4.jpg") no-repeat scroll bottom right;
}

.bg-attachment {
  height: 250px;
  box-shadow: 0 0 10px black;
  background: white url("img/image2.jpg") no-repeat fixed center;
}

.bg-size {
  box-shadow: 0 0 10px black;
  width: 500px;
  height: 300px;
  background-image: url("img/image2.jpg");
  background-size: cover;
}

.gradient {
  box-shadow: 0 0 10px black;
  width: 500px;
  height: 300px;
  background: linear-gradient(45deg, black, darkred);
}

```

You can check out the [Demo](https://praveenoruganti.github.io/praveenorugantitech-css/4_Background/Demo).

### [Buy me a Book](https://bit.ly/388sUbE)



