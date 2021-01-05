# CSS Selectors

In CSS, selectors are patterns used to select the element(s) you want to style.

![screenshot of the app](https://raw.githubusercontent.com/praveenorugantitech/praveenorugantitech-css/master/2_Selectors/images/css_selectors.png)

**HTML**

```HTML
<h1>First Heading</h1>
<h2 id="h2">Second Heading</h2>
<h3 class="h3">Third Heading</h3>
<h4>Fourth Heading</h3>
<div>
    <p>Child Selector</p>
    <h5>Five Heading </h5>
</div>
<div>
    <h6>Six Heading</h6>
</div>
<a href="https://www.google.com" target="_blank">Google</a>
```
**CSS**

```CSS
/* Universal selector */
* {
  background-color: limegreen;
}

/* Element selector */
body {
  margin: 0;
}

/* Grouping selector */
h1,
h4 {
  color: blue;
}

/* Id selector */
#h2 {
  color: brown;
}

/* Class selector */
.h3 {
  color: khaki;
}

/* Descendent selector */
div h6 {
  color: grey;
}

/* Child selector */
div > p {
  color: yellow;
  font-weight: bold;
}

/* Pseudo class selector */
a:hover {
  color: red;  
}

/* Pseudo element selector */
p::first-letter {
  color: black;
}

/* Attribute selector */
a[target="_blank"] {
  text-transform: uppercase;
}

```

You can check out the [Demo](https://praveenorugantitech.github.io/praveenorugantitech-css/2_Selectors/Demo).

<script data-name="BMC-Widget" src="https://cdnjs.buymeacoffee.com/1.0.0/widget.prod.min.js" data-id="praveenoruganti" data-description="Support me on Buy me a coffee!" data-message="Thank you for visiting. You can now buy me a coffee!" data-color="#5F7FFF" data-position="Right" data-x_margin="18" data-y_margin="18"></script>

