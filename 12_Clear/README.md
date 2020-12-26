# CSS Clear

CSS Clear property is used to stop next element to wrap around the adjacent floating elements. Clear can have clear left, clear right or clear both values.

CSS Clear Both property does not allow any element to wrap around any adjacent Floating element. Clear Left can stop wrapping around left floating element, Clear right can stop wrapping around right floating element. But Clear Both can stop wrapping around both left and right floating elements. It is compulsory to use clear both after floating elements.


Div tag is the preferred element to use clear both as div is block level.

clear: left | right | none | both;

- clear: right;    /*  Clear right floating only */
- clear: left;     /*  Clear left floating only */
- clear: none;     /*  Default */
- clear: both;     /*  Clear Both left & right floating */

**HTML**

```HTML
<div class="wrap">
    <div class="aside4">Aside 4</div>
    <div class="section4">Section 4</div>
    <div class="clear"></div>
    <p>This Paragraph will not wrap around Adjacent floating Divs as it is clear from both sides</p>
</div>
```

**CSS**

```CSS
* {
  margin: 0;
}
.wrap {
  width: 800px;
  border: 1px solid;
}
.aside4 {
  width: 200px;
  height: 200px;
  background: linear-gradient(45deg,black,blue);
  float: left;
}
.section4 {
  width: 600px;
  height: 200px;
  background: linear-gradient(45deg,black,limegreen);
  float: left;
}
.clear {
  clear: both;
}

```

You can check out the [Demo](https://praveenoruganti.github.io/praveenoruganti-css/12_Clear/Demo).

### [Buy me a Coffee](http://bit.ly/2WryDT8)
