


# Introduction to CSS



**What Is CSS?**

- CSS stands for Cascading Style Sheets.
- CSS describes how HTML elements are to be displayed on screen, on paper, or in other media.
- CSS saves a lot of work. It can control the layout of multiple web pages all at once.
- External stylesheets are stored in CSS files.
- CSS was introduced in 1996, so in the first few years of the Web, there was only HTML: [https://www.w3.org/TR/1999/REC-CSS1-19990111](https://www.w3.org/TR/1999/REC-CSS1-19990111)


**Why Use CSS?**

CSS is used to define styles for your web pages, including the design, layout, and variations in display for different devices and screen sizes.

**CSS Syntax**

A CSS rule-set consists of a selector and a declaration block:

![screenshot of the app](https://raw.githubusercontent.com/praveenorugantitech/praveenorugantitech-css/master/0_Introduction/images/screenshot.PNG)


- The selector points to the HTML element you want to style.
- The declaration block contains one or more declarations separated by semicolons.
- Each declaration includes a CSS property name and a value, separated by a colon.
- Multiple CSS declarations are separated by semicolons. 
- Declaration blocks are surrounded by curly braces.
- In this example, all p tag elements will be center-aligned, with a red text color:
```CSS
    p {
    color: red;
    text-align: center;
    }
```