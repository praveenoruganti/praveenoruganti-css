# CSS Flex Box

**Why Flex Box?**

The Flexible Box Layout(Flex Box) provides many ways for aligning content, ordering items, and implementing flexible sizing.

Flex Box is one dimensional layout i.e.. items are laid out on a single axis, either columns or rows.

In order to get Flex Box to work, we need to establish parent-child relationship. The parent is flex container and everything within it is the children or flex items.

![screenshot of the app](https://raw.githubusercontent.com/praveenoruganti/praveenoruganti-css/master/14_Flex_Box/images/Flex_Box.PNG)


The Flex Box Layout (Flexible Box) module aims at providing a more efficient way to layout,align and distribute space among items in a container, even when their size is unknown
and/or dynamic (thus the word "flex").

The main idea behind the flex layout is to give the container the ability to alter its items width/height (and order) to best fill the available space (mostly to accommodate to all kind
of display devices and screen sizes). A flex container expands items to fill available free space or shrinks them to prevent overflow.

Most importantly, the flex Box layout is direction-agnostic as opposed to the regular layouts (block which is vertically-based and inline which is horizontally-based).While those work well
for pages, they lack flexibility (no pun intended) to support large or complex applications (especially when it comes to orientation changing, resizing, stretching, shrinking, etc.).

Note: Flex Box layout is most appropriate to the components of an application, and small-scale layouts, while the Grid layout is intended for larger scale layouts.

If regular layout is based on both block and inline flow directions,the flex layout is based on flex-flow directions.

**Properties for the Parent(flex container)**

- **display**
This defines a flex container; inline or block depending on the given value.
It enables a flex context for all its direct children.<br/>
**display: flex; or display: inline-flex;**<br/>
Note that CSS columns have no effect on a flex container.

- **flex-direction**
This establishes the main-axis, thus defining the direction flex items are placed in the flex container.<br/>
Flex Box is (aside from optional wrapping) a single-direction layout concept. <br/>
Think of flex items as primarily laying out either in horizontal rows or vertical columns.<br/>
**flex-direction: row (or) row-reverse (or) column (or) column-reverse;**<br/>
row (default): left to right in ltr; right to left in rtl<br/>
row-reverse: right to left in ltr; left to right in rtl<br/>
column: same as row but top to bottom<br/>
column-reverse: same as row-reverse but bottom to top

- **flex-wrap**
By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.<br/>
**flex-wrap: nowrap (or) wrap (or) wrap-reverse;**<br/>
nowrap (default): all flex items will be on one line<br/>
wrap: flex items will wrap onto multiple lines, from top to bottom.<br/>
wrap-reverse: flex items will wrap onto multiple lines from bottom to top.

- **flex-flow**
This is a shorthand for the flex-direction and flex-wrap properties, which together
define the flex container's main and cross axes. The default value is row nowrap.<br/>
**flex-flow: column wrap;**

- **justify-content**
This defines the alignment along the main axis. It helps distribute extra free space
leftover when either all the flex items on a line are inflexible, or are flexible
but have reached their maximum size. It also exerts some control over the alignment
of items when they overflow the line.

**justify-content: flex-start (or) flex-end (or) center (or) space-between (or) space-around (or) space-evenly (or) start (or) end (or) left (or) right ... + safe (or) unsafe;**

a) **flex-start (default)**: items are packed toward the start of the flex-direction.<br/>
b) **flex-end**: items are packed toward the end of the flex-direction.<br/>
c) **start**: items are packed toward the start of the writing-mode direction.<br/>
d) **end**: items are packed toward the end of the writing-mode direction.<br/>
e) **left**: items are packed toward left edge of the container, unless that doesn't make sense with the flex-direction, then it behaves like start.<br/>
f) **right**: items are packed toward right edge of the container, unless that doesn't make sense with the flex-direction, then it behaves like start.<br/>
g) **center**: items are centered along the line<br/>
h) **space-between**: items are evenly distributed in the line; first item is on the start line , last item on the end line<br/>
i) **space-around**: items are evenly distributed in the line with equal space around them.
  Note that visually the spaces aren't equal, since all the items have equal space on both sides.<br/>
  The first item will have one unit of space against the container edge, but two units of space between the next item because that next item has its own spacing that applies.<br/>
j) **space-evenly**: items are distributed so that the spacing between any two items(and the space to the edges) is equal.

- **align-items**
This defines the default behavior for how flex items are laid out along the cross axis
on the current line. Think of it as the justify-content version for the cross-axis
(perpendicular to the main-axis).

**align-items: stretch (or) flex-start (or) flex-end (or) center (or) baseline (or) first baseline (or) last baseline (or) start (or) end (or) self-start (or) self-end + ... safe (or) unsafe;**

a) **stretch (default)**: stretch to fill the container (still respect min-width/max-width)<br/>
b) **flex-start / start / self-start**: items are placed at the start of the cross axis. The difference between these is subtle, and is about respecting the flex-direction rules or the writing-mode rules.<br/>
c) **flex-end / end / self-end**: items are placed at the end of the cross axis. The difference again is subtle and is about respecting flex-direction rules vs. writing-mode rules.<br/>
d) **center**: items are centered in the cross-axis<br/>
e)**baseline**: items are aligned such as their baselines align

- **align-content**
This aligns a flex container's lines within when there is extra space in the cross-axis,
similar to how justify-content aligns individual items within the main-axis.
**Note**: this property has no effect when there is only one line of flex items.

**align-content: flex-start (or) flex-end (or) center (or) space-between (or) space-around (or) space-evenly (or) stretch (or) start (or) end (or) baseline (or) first baseline (or) last baseline + ... safe (or) unsafe;**

a) **flex-start / start**: items packed to the start of the container. The (more supported)
flex-start honors the flex-direction while start honors the writing-mode direction.<br/>
b) **flex-end / end**: items packed to the end of the container. The (more support)
flex-end honors the flex-direction while end honors the writing-mode direction.<br/>
c) **center**: items centered in the container<br/>
d) **space-between**: items evenly distributed; the first line is at the start of the
container while the last one is at the end<br/>
e) **space-around**: items evenly distributed with equal space around each line<br/>
g) **space-evenly**: items are evenly distributed with equal space around them<br/>
h) **stretch (default)**: lines stretch to take up the remaining space


**Properties for the Children(flex items)**
- **order**
By default, flex items are laid out in the source order. However, the order property controls
the order in which they appear in the flex container.

**order: 5; (default is 0)**

- **flex-grow**
This defines the ability for a flex item to grow if necessary. It accepts a unit less value
that serves as a proportion. It dictates what amount of the available space inside the
flex container the item should take up.

If all items have flex-grow set to 1, the remaining space in the container will be
distributed equally to all children. If one of the children has a value of 2,
the remaining space would take up twice as much space as the others
(or it will try to, at least).

**flex-grow: 4; (default is 0)**<br/>
Negative numbers are invalid.

- **flex-shrink**
This defines the ability for a flex item to shrink if necessary.

**flex-shrink: 3; (default is 1)**<br/>
Negative numbers are invalid.

- **flex-basis**
This defines the default size of an element before the remaining space is distributed.
It can be a length (e.g. 20%, 5rem, etc.) or a keyword. The auto keyword means
"look at my width or height property" (which was temporarily done by the main-size keyword
until deprecated). The content keyword means "size it based on the item's content"
this keyword isn't well supported yet, so it's hard to test and harder to know what
its brethren max-content, min-content, and fit-content do.

**flex-basis:  <width> (or) auto; ( default is auto)**<br/>
If set to 0, the extra space around content isn't factored in. If set to auto,
the extra space is distributed based on its flex-grow value.

- **flex**
This is the shorthand for flex-grow, flex-shrink and flex-basis combined.
The second and third parameters (flex-shrink and flex-basis) are optional.
The default is 0 1 auto, but if you set it with a single number value, it's like 1 0.

**flex: none (or) [ <'flex-grow'> <'flex-shrink'>? (or) <'flex-basis'> ]**

It is recommended that you use this shorthand property rather than set the individual properties.
The shorthand sets the other values intelligently.

- **align-self**
This allows the default alignment (or the one specified by align-items) to be overridden
for individual flex items.

**align-self: auto (or) flex-start (or) flex-end (or) center (or) baseline (or) stretch;**<br/>
Note that float, clear and vertical-align have no effect on a flex item

**HTML**
```HTML
<h2>Flex Box with flex direction : row</h2>
<div class="flexContainer1">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
</div>
<h2>Flex Box with flex direction : row reverse</h2>
<div class="flexContainer2">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
</div>
<h2>Flex Box with flex direction : column</h2>
<div class="flexContainer3">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
</div>
<h2>Flex Box with flex direction : column reverse</h2>
<div class="flexContainer4">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
</div>
<h2>Flex Box with flex wrap : no wrap</h2>
<div class="flexContainer5">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
    <div class="flexItem">5</div>
    <div class="flexItem">6</div>
    <div class="flexItem">7</div>
    <div class="flexItem">8</div>
    <div class="flexItem">9</div>
    <div class="flexItem">10</div>
</div>
<h2>Flex Box with flex wrap : wrap</h2>
<div class="flexContainer6">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
    <div class="flexItem">5</div>
    <div class="flexItem">6</div>
    <div class="flexItem">7</div>
    <div class="flexItem">8</div>
    <div class="flexItem">9</div>
    <div class="flexItem">10</div>
</div>
<h2>Flex Box with flex wrap : wrap-reverse</h2>
<div class="flexContainer7">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
    <div class="flexItem">5</div>
    <div class="flexItem">6</div>
    <div class="flexItem">7</div>
    <div class="flexItem">8</div>
    <div class="flexItem">9</div>
    <div class="flexItem">10</div>
</div>
<h2>Flex Box with justify content: flex-start</h2>
<div class="flexContainer8">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
</div>
<h2>Flex Box with justify content: flex-end</h2>
<div class="flexContainer9">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
</div>
<h2>Flex Box with justify content: center</h2>
<div class="flexContainer10">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
</div>
<h2>Flex Box with justify content: space-between</h2>
<div class="flexContainer11">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
</div>
<h2>Flex Box with justify content: space-around</h2>
<div class="flexContainer12">
    <div class="flexItem">1</div>
    <div class="flexItem">2</div>
    <div class="flexItem">3</div>
    <div class="flexItem">4</div>
</div>
<h2>Flex Box with order</h2>
<div class="flexContainer1">
    <div class="flexItem one">1</div>
    <div class="flexItem two">2</div>
    <div class="flexItem three">3</div>
    <div class="flexItem four">4</div>
</div>
<h2>Flex Box with flex grow</h2>
<div class="flexContainer1">
    <div class="flexItem five">5</div>
    <div class="flexItem six">6</div>
    <div class="flexItem seven">7</div>
    <div class="flexItem eight">8</div>
</div>
```

**CSS**

```CSS
.flexContainer1 {
  display: flex;
  flex-direction: row;
}

.flexItem {
  width: 10%;
  margin: 10px;
  padding: 10px;
  border: 20px solid darkred;
  font-weight: bold;
  font-size: 40px;
}

.flexContainer2 {
  display: flex;
  flex-direction: row-reverse;
}

.flexContainer3 {
  display: flex;
  flex-direction: column;
}

.flexContainer4 {
  display: flex;
  flex-direction: column-reverse;
}

.flexContainer5 {
  display: flex;
  flex-wrap: nowrap;
}

.flexContainer6 {
  display: flex;
  flex-wrap: wrap;
}

.flexContainer7 {
  display: flex;
  flex-wrap: wrap-reverse;
}

.flexContainer8 {
  display: flex;
  justify-content: flex-start;
}

.flexContainer9 {
  display: flex;
  justify-content: flex-end;
}

.flexContainer10 {
  display: flex;
  justify-content: center;
}

.flexContainer11 {
  display: flex;
  justify-content: space-between;
}

.flexContainer12 {
  display: flex;
  justify-content: space-around;
}

.one {
  order: 2;
}

.two {
  order: 3;
}

.three {
  order: 4;
}

.four {
  order: 1;
}

.five {
  flex-grow: 1;
}

.six {
  flex-grow: 2;
}

.eight {
  flex-grow: 4;
}

```

You can check out the [Demo](https://praveenoruganti.github.io/praveenoruganti-css/14_Flex_Box/Demo).

You can check out the [Flex Box Examples](https://praveenoruganti.github.io/praveenoruganti-css/14_Flex_Box/Demo/Examples.html).

### [Buy me a Book](https://www.buymeacoffee.com/praveenoruganti)

