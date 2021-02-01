


# CSS Referencing



There are 3 types of CSS Referencing.

- External CSS with <link>

**HTML**

```html
<link rel="stylesheet" href="styles.css" />
```
**CSS**

```css
h1{
    color:red;
}
```
- Inline CSS and it has highest priority and will override external and internal styles and browser defaults

```html
<h2 style="color:green">Second Heading</h2>
```
- Internal CSS  is better than inline CSS but its not a best practice to use.

```html
<style>
    h3 {
        color: blue;
    }
</style>
```

You can check out the [Demo](https://praveenorugantitech.github.io/praveenorugantitech-css-course/1_Referencing/Demo){:target="_blank"}




