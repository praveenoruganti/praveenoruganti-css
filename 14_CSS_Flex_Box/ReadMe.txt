CSS Flex Box

The Flexbox Layout (Flexible Box) module aims at providing a more efficient way to layout,
align and distribute space among items in a container, even when their size is unknown 
and/or dynamic (thus the word "flex").

The main idea behind the flex layout is to give the container the ability to alter its items
width/height (and order) to best fill the available space (mostly to accommodate to all kind 
of display devices and screen sizes). A flex container expands items to fill available 
free space or shrinks them to prevent overflow.

Most importantly, the flexbox layout is direction-agnostic as opposed to the regular layouts 
(block which is vertically-based and inline which is horizontally-based).While those work well 
for pages, they lack flexibility (no pun intended) to support large or complex applications 
(especially when it comes to orientation changing, resizing, stretching, shrinking, etc.).

Note: Flexbox layout is most appropriate to the components of an application, and small-scale 
layouts, while the Grid layout is intended for larger scale layouts.

If regular layout is based on both block and inline flow directions, 
the flex layout is based on flex-flow directions.


Properties for the Parent(flex container)

1. display
This defines a flex container; inline or block depending on the given value. 
It enables a flex context for all its direct children.
display: flex; or display: inline-flex;
Note that CSS columns have no effect on a flex container.

2. flex-direction
This establishes the main-axis, thus defining the direction flex items are placed in the 
flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. 
Think of flex items as primarily laying out either in horizontal rows or vertical columns.
flex-direction: row | row-reverse | column | column-reverse;
row (default): left to right in ltr; right to left in rtl
row-reverse: right to left in ltr; left to right in rtl
column: same as row but top to bottom
column-reverse: same as row-reverse but bottom to top

3. flex-wrap
By default, flex items will all try to fit onto one line. You can change that and allow 
the items to wrap as needed with this property.
flex-wrap: nowrap | wrap | wrap-reverse;
nowrap (default): all flex items will be on one line
wrap: flex items will wrap onto multiple lines, from top to bottom.
wrap-reverse: flex items will wrap onto multiple lines from bottom to top.

4. flex-flow
This is a shorthand for the flex-direction and flex-wrap properties, which together 
define the flex container’s main and cross axes. The default value is row nowrap.
flex-flow: column wrap;

5. justify-content
This defines the alignment along the main axis. It helps distribute extra free space 
leftover when either all the flex items on a line are inflexible, or are flexible 
but have reached their maximum size. It also exerts some control over the alignment 
of items when they overflow the line.

justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly 
| start | end | left | right ... + safe | unsafe;

a) flex-start (default): items are packed toward the start of the flex-direction.
b) flex-end: items are packed toward the end of the flex-direction.
c) start: items are packed toward the start of the writing-mode direction.
d) end: items are packed toward the end of the writing-mode direction.
e) left: items are packed toward left edge of the container, unless that doesn’t make sense 
with the flex-direction, then it behaves like start.
f) right: items are packed toward right edge of the container, unless that doesn’t make sense 
with the flex-direction, then it behaves like start.
g) center: items are centered along the line
h) space-between: items are evenly distributed in the line; first item is on the start line
, last item on the end line
i) space-around: items are evenly distributed in the line with equal space around them. 
Note that visually the spaces aren’t equal, since all the items have equal space on both sides. 
The first item will have one unit of space against the container edge, but two units 
of space between the next item because that next item has its own spacing that applies.
j) space-evenly: items are distributed so that the spacing between any two items
 (and the space to the edges) is equal.

6. align-items
This defines the default behavior for how flex items are laid out along the cross axis 
on the current line. Think of it as the justify-content version for the cross-axis 
(perpendicular to the main-axis).

align-items: stretch | flex-start | flex-end | center | baseline | first baseline 
| last baseline | start | end | self-start | self-end + ... safe | unsafe;

a) stretch (default): stretch to fill the container (still respect min-width/max-width)
b) flex-start / start / self-start: items are placed at the start of the cross axis. The difference between these is subtle, and is about respecting the flex-direction rules or the writing-mode rules.
c) flex-end / end / self-end: items are placed at the end of the cross axis. The difference again is subtle and is about respecting flex-direction rules vs. writing-mode rules.
d) center: items are centered in the cross-axis
e)baseline: items are aligned such as their baselines align

7. align-content
This aligns a flex container’s lines within when there is extra space in the cross-axis, 
similar to how justify-content aligns individual items within the main-axis.
Note: this property has no effect when there is only one line of flex items.

align-content: flex-start | flex-end | center | space-between | space-around | space-evenly 
| stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;

a) flex-start / start: items packed to the start of the container. The (more supported) 
flex-start honors the flex-direction while start honors the writing-mode direction.
b) flex-end / end: items packed to the end of the container. The (more support) 
flex-end honors the flex-direction while end honors the writing-mode direction.
c) center: items centered in the container
d) space-between: items evenly distributed; the first line is at the start of the 
container while the last one is at the end
e) space-around: items evenly distributed with equal space around each line
g) space-evenly: items are evenly distributed with equal space around them
h) stretch (default): lines stretch to take up the remaining space


Properties for the Children(flex items)
1. order
By default, flex items are laid out in the source order. However, the order property controls 
the order in which they appear in the flex container.
order: 5; (default is 0)

2. flex-grow
This defines the ability for a flex item to grow if necessary. It accepts a unitless value 
that serves as a proportion. It dictates what amount of the available space inside the 
flex container the item should take up.

If all items have flex-grow set to 1, the remaining space in the container will be 
distributed equally to all children. If one of the children has a value of 2, 
the remaining space would take up twice as much space as the others 
(or it will try to, at least).

flex-grow: 4; (default is 0)
Negative numbers are invalid.

3. flex-shrink
This defines the ability for a flex item to shrink if necessary.

flex-shrink: 3; (default is 1)
Negative numbers are invalid.

4. flex-basis
This defines the default size of an element before the remaining space is distributed. 
It can be a length (e.g. 20%, 5rem, etc.) or a keyword. The auto keyword means 
"look at my width or height property" (which was temporarily done by the main-size keyword 
until deprecated). The content keyword means "size it based on the item’s content" – 
this keyword isn’t well supported yet, so it’s hard to test and harder to know what 
its brethren max-content, min-content, and fit-content do.

flex-basis:  | auto; ( default is auto)
If set to 0, the extra space around content isn’t factored in. If set to auto, 
the extra space is distributed based on its flex-grow value.

5. flex
This is the shorthand for flex-grow, flex-shrink and flex-basis combined. 
The second and third parameters (flex-shrink and flex-basis) are optional. 
The default is 0 1 auto, but if you set it with a single number value, it’s like 1 0.

flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]

It is recommended that you use this shorthand property rather than set the individual properties. 
The shorthand sets the other values intelligently.

6. align-self
This allows the default alignment (or the one specified by align-items) to be overridden 
for individual flex items.

align-self: auto | flex-start | flex-end | center | baseline | stretch;

Note that float, clear and vertical-align have no effect on a flex item


