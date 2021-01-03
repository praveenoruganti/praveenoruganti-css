# CSS Position

Here with the CSS Position Properties.

- **static**  default position of any html element (static).
- **relative** This is positioned relative to its own.
- **absolute** This is positioned relative to its parent.
- **fixed** This is to fix an element in the given position.
- **sticky** This is to stick any element in the given position.

Supporting properties for CSS Position are top,right,bottom,left.

**HTML**

```HTML
<div class="box box1"></div>
<div class="container">
    <div class="box box2"></div>
    <div class="box box3"></div>
</div>
<div class="box box4"></div>
<div class="box box5"></div>

```

**CSS**

```CSS

body {
  height: 5000px;
}
.box {
  width: 100px;
  height: 100px;
  box-shadow: 0 0 5px black;
}

.box1 {
  background-color: red;
  position: relative;
  left: 200px;
}

.container {
  width: 500px;
  height: 500px;
  background-color: rgba(0, 0, 0, 0.5);
  position: relative;
  left: 400px;
}

.box2 {
  background-color: green;
  position: absolute;
  left: 100px;
  top: 100px;
}

.box3 {
  background-color: blue;
  position: absolute;
  right: 100px;
  bottom: 100px;
}

.box4 {
  background-color: yellow;
  position: fixed;
  top: 300px;
  right: 10%;
}

.box5 {
  background-color: brown;
  position: sticky;
  top: 0;
}

```

You can check out the [Demo](https://praveenoruganti.github.io/praveenoruganti-css/8_Position/Demo).

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

