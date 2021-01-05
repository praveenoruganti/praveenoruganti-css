# CSS Referencing

There are 3 types of CSS Referencing.

- External CSS with <link>

**HTML**

```HTML
<link rel="stylesheet" href="styles.css" />
```
**CSS**

```CSS
h1{
    color:red;
}
```
- Inline CSS and it has highest priority and will override external and internal styles and browser defaults

```HTML
<h2 style="color:green">Second Heading</h2>
```
- Internal CSS  is better than inline CSS but its not a best practice to use.

```HTML
<style>
    h3 {
        color: blue;
    }
</style>
```

You can check out the [Demo](https://praveenorugantitech.github.io/praveenorugantitech-css/1_Referencing/Demo).


<script data-name="BMC-Widget" src="https://cdnjs.buymeacoffee.com/1.0.0/widget.prod.min.js" data-id="praveenoruganti" data-description="Support me on Buy me a coffee!" data-message="Thank you for visiting. You can now buy me a coffee!" data-color="#5F7FFF" data-position="Right" data-x_margin="18" data-y_margin="18"></script>

