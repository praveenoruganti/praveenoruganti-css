


# CSS Font



Here with the CSS Font properties.

- **font-family**  Defines a list of fonts for element.
- **font-style**  Defines the font style for the text.
- **font-weight**  Specify the font weight of the text.
- **font-size**  Defines the font size for the text.
- **font-variant**  Specify the font variant.
- **font-size-adjust**  Preserves the readability of text when font fallback occurs.
- **font-stretch**  Selects a normal, condensed, or expanded face from a font.
- **Shorthand Property**  font: style variant weight size/line-height family

**HTML**

```html
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

```css
p {
  font-style: italic;
  font-variant: small-caps;
  font-weight: bold;
  font-size: 25px;
  font-family: Arial, Helvetica, sans-serif;
  font-stretch: condensed;
}

p.b {
  font: italic small-caps bold 25px Arial, Helvetica, sans-serif;
}

```

You can check out the [Demo](https://praveenorugantitech.github.io/praveenorugantitech-css-course/6_Font/Demo){:target="_blank"}.





