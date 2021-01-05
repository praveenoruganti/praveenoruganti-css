# CSS Text

Here with the CSS Text Properties.

**CSS Text**  properties that allows you to define various text styles such as
color, alignment, spacing, decoration, transformation, etc.

- **color**  property is used to set the color of the text.
- **text-align**  Sets the horizontal alignment of inline content.
- **direction**  Define the text direction/writing direction.
- **vertical-align**  Sets the vertical positioning of an element relative to the current text baseline.
- **text-decoration**  Specifies the decoration added to text.
- **text-transform**  Transforms the case of the text.
- **text-indent**  Indent the first line of text.
- **line-height**  Sets the height between lines of text.
- **letter-spacing**  Sets the extra spacing between letters.
- **word-spacing**  Sets the spacing between words.
- **white-space**  Specifies how white space inside the element is handled.
- **text-shadow**  Applies one or more shadows to the text content of an element.

**HTML**

```HTML

<h1>Sample Text</h1>
<p>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
    incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
    nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore
    eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident,
    sunt in culpa qui officia deserunt mollit anim id est laborum.
</p> <br />

<p class="b">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
    incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
    nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore
    eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident,
    sunt in culpa qui officia deserunt mollit anim id est laborum.
</p>

```

**CSS**

```CSS

p {
  color: darkred;
}

h1 {
  text-align: center;
}

.b {
  direction: rtl;
  text-transform: uppercase;
  color: blue;
  text-indent: 1vh;
  line-height: 150%;
  letter-spacing: 5px;
  word-spacing: 5px;
  white-space: pre;
  text-shadow: 1px 1px red;
}

```

You can check out the [Demo](https://praveenoruganti.github.io/praveenorugantitech-css/7_Text/Demo).


### [Buy me a Book](https://bit.ly/388sUbE)

