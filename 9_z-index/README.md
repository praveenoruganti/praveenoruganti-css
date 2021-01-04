# CSS z-index

The z-index property specifies the stack order of an element.

An element with greater stack order is always in front of an element with a lower stack order.

**Note**: z-index only works on positioned elements (position: absolute, position: relative, position: fixed, or position: sticky).


**HTML**

```HTML
<div class="main">
    <div class="common one">One</div>
    <div class="common two">Two</div>
    <div class="common three">Three</div>
    <div class="common four">Four</div>
    <div class="common five">Five</div>
    <div class="common six">Six</div>
</div>
```

**CSS**

```CSS

body {
  font-family: "Courier New", Courier, monospace;
  margin: 0;
}

.main {
  margin: 0 auto;
}

.common {
  width: 200px;
  height: 200px;
  color: grey;
  border: 1px solid limegreen;
  position: absolute;
  color: black;
  font-weight: bold;
}

.one {
  background-color: red;
  z-index: 0;
  left: 20px;
  top: 40px;
}

.two {
  background-color: green;
  z-index: 1;
  left: 40px;
  top: 80px;
}

.three {
  background-color: blue;
  z-index: 2;
  left: 60px;
  top: 120px;
}

.four {
  background-color: brown;
  z-index: 3;
  left: 80px;
  top: 160px;
}

.five {
  background-color: deeppink;
  z-index: 4;
  left: 100px;
  top: 200px;
}

.six {
  background-color: yellow;
  z-index: 5;
  left: 120px;
  top: 240px;
}

```

You can check out the [Demo](https://praveenoruganti.github.io/praveenoruganti-css/9_z-index/Demo).


### [Buy me a Book](https://bit.ly/388sUbE)


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
