# CSS Selectors

In CSS, selectors are patterns used to select the element(s) you want to style.

![screenshot of the app](https://raw.githubusercontent.com/praveenoruganti/praveenoruganti-css/master/2_Selectors/images/css_selectors.png)

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

You can check out the [Demo](https://praveenoruganti.github.io/praveenoruganti-css/2_Selectors/Demo).

### [Buy me a Book](https://www.buymeacoffee.com/praveenoruganti)


### Connect with me:

[<img align="left" alt="praveenorugantitech.blogspot.com" width="22px" src="https://raw.githubusercontent.com/iconic/open-iconic/master/svg/globe.svg" />][website]
[<img align="left" alt="praveenoruganti | Facebook Group" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/facebook.svg" />][facebookgroup]
[<img align="left" alt="praveenoruganti | Twitter" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/twitter.svg" />][twitter]
[<img align="left" alt="praveenoruganti | Instagram" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/instagram.svg" />][instagram]
[<img align="left" alt="praveenoruganti | Email" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/gmail.svg" />][email]

<br/>

[website]: https://praveenorugantitech.blogspot.com
[twitter]: https://mobile.twitter.com/praveenoruganti
[facebookgroup]: https://www.facebook.com/groups/praveenorugantitech
[instagram]: https://instagram.com/praveenorugantitech
[email]: mailto:praveenorugantitech@gmail.com

