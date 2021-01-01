# CSS Display

Here with the CSS Display Properties.

- display: inline
- display: block
- display: none
- display: inline-block
- display: flex


![screenshot of the app](https://raw.githubusercontent.com/praveenoruganti/praveenoruganti-css/master/10_Display/images/Display.PNG)


**HTML**

```HTML
<!-- inline -->
<div>
    <h2>Good Morning</h2>
    <h2>Good Afternoon</h2>
    <h2>Good Evening</h2>
</div>
<!-- block -->
<div>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
        <span>1.et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco </span>
        <span>2.laboris nisi utaliquip ex ea commodo consequat. Duis aute irure dolor in</span>
        <span>3.reprehenderit in voluptatevelit esse cillum dolore eu fugiat nulla pariatur. </span>
        <span>4.Excepteur sint occaecat cupidatat non
            proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</span></p>
</div>
<!-- block -->
<div>
    <a href="#">Home</a>
    <a href="#">About Us</a>
    <a href="#">Courses</a>
    <a href="#">Contact Us</a>
</div>
<!-- Hide -->
<div>
    <h1>Hello I am Hidden</h1>
</div>

<!-- Inline Block-->
<div class="parent">

    <div class="child">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
            ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
            fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
            deserunt mollit anim id est laborum.</p>
    </div>
    <div class="child">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
            ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
            fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
            deserunt mollit anim id est laborum.</p>
    </div>
    <div class="child">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
            ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
            fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
            deserunt mollit anim id est laborum.</p>
    </div>
    <div class="child">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
            ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
            fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
            deserunt mollit anim id est laborum.</p>
    </div>

</div>

```

**CSS**

```CSS

body {
  font-family: "Courier New", Courier, monospace;
}

div {
  margin: 20px;
}

h2 {
  background: lightsalmon;
  padding: 5px;
  margin: 5px;
  display: inline;
}

span {
  display: block;
  background: orange;
}

a {
  display: block;
  background: limegreen;
  padding: 5px;
  margin: 5px;
  color: white;
  width: 100px;
}

h1 {
  background-color: brown;
  color: white;
  text-align: center;
  padding: 20px;
  display: none;
}

.parent {
  background: lightgreen;
  padding: 15px;
  text-align: center;
}

.child {
  background: black;
  color: whitesmoke;
  width: 200px;
  padding: 15px;
  display: inline-block;
  box-shadow: 0 0 10px black;
}

```

You can check out the [Demo](https://praveenoruganti.github.io/praveenoruganti-css/10_Display/Demo).


