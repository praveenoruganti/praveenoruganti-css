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

You can check out the [Demo](https://praveenorugantitech.github.io/praveenorugantitech-css/8_Position/Demo).

### [Buy me a Book](https://bit.ly/388sUbE)



