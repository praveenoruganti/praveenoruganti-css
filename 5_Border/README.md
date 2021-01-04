# CSS Border

Here with the CSS Border properties.

- **border-width** Thickness of border, we can give values in px,cm,mm.
- **border-style** solid, dotted, dashed, double
- **border-color** text, hex, rgb
- **border** width style color
  a) border-left: width style color
  b) border-right: width style color
  c) border-top: width style color
  d) border-bottom: width style color
- **border-radius** px or %
  border-radius: TL TR BR BL;

If border-color is omitted, the color applied will be the color of the text.

**HTML**

```HTML
<h2> Border All Sides with solid style</h2>
<div class="border-all-solid">
    <h2>Border All Sides</h2>
</div>
<h2> Border All Sides with dotted style</h2>
<div class="border-all-dotted">
    <h2>Border All Sides</h2>
</div>
<h2> Border All Sides with dashed style</h2>
<div class="border-all-dashed">
    <h2>Border All Sides</h2>
</div>
<h2> Border All Sides with double style</h2>
<div class="border-all-double">
    <h2>Border All Sides</h2>
</div>
<h2> Border left side with double style</h2>
<div class="border-left-double">
    <h2>Border left Side</h2>
</div>
<h2> Border right side with double style</h2>
<div class="border-right-double">
    <h2>Border right Side</h2>
</div>
<h2> Border top side with double style</h2>
<div class="border-top-double">
    <h2>Border top Side</h2>
</div>
<h2> Border bottom side with double style</h2>
<div class="border-bottom-double">
    <h2>Border bottom Side</h2>
</div>
<h2> Border Rounded All Sides with solid style</h2>
<div class="border-rounded-all-solid">
    <h2>Border Rounded All Sides</h2>
</div>
<h2> Border Rounded two sides with solid style</h2>
<div class="border-rounded-two-solid">
    <h2>Border Rounded two sides</h2>
</div>
<h2>Circle</h2>
<section class="circle"></section>
<h2>Border Circle</h2>
<section class="border-circle"></section>
<h2>Border Frame</h2>
<section class="border-frame"></section>
<h2>Border Ring</h2>
<section class="border-ring"></section>
<h2>Custom Border</h2>
<section class="custom-border">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/NBe7fzCK2V0" frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen>
    </iframe>
</section>

```

**CSS**

```CSS

body {
  font-family: "Courier New", Courier, monospace;
  margin: 0;
  padding: 10px;
}

div {
  background: lightgreen;
  text-align: center;
  padding: 20px;
  font-size: 25px;
  width: 800px;
  padding: 10px;
}

.border-all-solid {
  border: 15px solid black;
}

.border-all-dotted {
  border: 15px dotted black;
}

.border-all-dashed {
  border: 15px dashed black;
}

.border-all-double {
  border: 15px double black;
}

.border-left-double {
  border-left: 15px double black;
}

.border-right-double {
  border-right: 15px double black;
}

.border-top-double {
  border-top: 15px double black;
}

.border-bottom-double {
  border-bottom: 15px double black;
}

.border-rounded-all-solid {
  border: 15px solid black;
  border-radius: 50px;
}

.border-rounded-two-solid {
  border: 15px solid black;
  border-radius: 60px 0 60px 0;
}

.circle {
  height: 200px;
  width: 200px;
  box-shadow: 0 0 10px black;
  border-radius: 50%;
  background: lightgreen;
  padding: 10px;
}

.border-circle {
  height: 200px;
  width: 200px;
  box-shadow: 0 0 10px black;
  border-radius: 50%;
  background: lightgreen;
  border: 25px solid black;
  padding: 10px;
}

.border-frame {
  height: 200px;
  width: 200px;
  box-shadow: 0 0 10px black;
  border-top: 25px solid black;
  border-bottom: 25px solid black;
  border-left: 35px solid limegreen;
  border-right: 35px solid limegreen;
  padding: 10px;
}

.border-ring {
  height: 200px;
  width: 200px;
  box-shadow: 0 0 10px black;
  border-radius: 50%;
  border-top: 25px solid black;
  border-bottom: 25px solid black;
  border-left: 35px solid limegreen;
  border-right: 35px solid limegreen;
  background: linear-gradient(45deg, green, yellow);
  padding: 10px;
}

.custom-border {
  height: 315px;
  width: 560px;
  box-shadow: 0 0 10px black;
  border-top: 25px solid black;
  border-bottom: 25px solid black;
  border-left: 35px solid limegreen;
  border-right: 35px solid limegreen;
}

```

You can check out the [Demo](https://praveenoruganti.github.io/praveenoruganti-css/5_Border/Demo).


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
