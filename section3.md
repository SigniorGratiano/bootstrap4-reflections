## Section 3 Reflections

### _15. Buttons and Button Groups_

Buttons:
```html
<button class="btn btn-primary" type="button">Primary</button>
<button class="btn btn-secondary" type="button">Secondary</button>
<button class="btn btn-success" type="button">Success</button>
<button class="btn btn-info" type="button">Info</button>
<button class="btn btn-warning" type="button">Warning</button>
<button class="btn btn-danger" type="button">Danger</button>
<button class="btn btn-light" type="button">Light</button>
<button class="btn btn-dark" type="button">Dark</button>
<button class="btn btn-link">a button that looks like a link</button>
```

We can add 'btn' classes to:
```html
<a class="btn" href="#" role="button">Link</a>
<button class="btn" type="submit">Button</button>
<input class="btn" type="button" value="Input">
<input class="btn" type="submit" value="Submit">
<input class="btn" type="reset" value="Reset">
```

Outline buttons:
```html
<button class="btn btn-outline-primary" type="button">Primary Outline</button>
<button class="btn btn-outline-secondary" type="button">Secondary Outline</button>
<button class="btn btn-outline-success" type="button">Success Outline</button>
<button class="btn btn-outline-info" type="button">Info Outline</button>
<button class="btn btn-outline-warning" type="button">Warning Outline</button>
<button class="btn btn-outline-danger" type="button">Danger Outline</button>
<button class="btn btn-outline-light" type="button">Light Outline</button>
<button class="btn btn-outline-dark" type="button">Dark Outline</button>
```

Button sizes:
```html
<button class="btn btn-lg" type="button">Large button</button>
<button class="btn btn-sm" type="button">Small button</button>
<button class="btn btn-block" type="button">Block level button</button>
```

Button states:
```html
<button class="btn" type="button">Regular Button</button>
<button class="btn active" type="button">Active Button</button>
<button class="btn disabled" type="button">Disabled Button</button>
<button class="btn" type="button" data-toggle="button">
    Toggle State - the button toggles between regular and active colors when clicked
</button>
```

Button dropdowns:
```html
<div class="dropdown">
    <button class="btn dropdown-toggle" type="button"
    data-toggle="dropdown">
        My Dropdown
    </button>
    <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Link One</a>
        <a class="dropdown-item" href="#">Link Two</a>
        <a class="dropdown-item" href="#">Link Three</a>
    </div>
</div>
```

Split dropdowns:
```html
<div class="btn-group">
    <button class="btn" type="button">My Button</button>
    <button class="btn dropdown-toggle" type="button"
    data-toggle="dropdown">
        <span>Toggle Dropdown</span>
    </button>
    <div class="dropdown-menu">
      <a class="dropdown-item" href="#">Link One</a>
      <a class="dropdown-item" href="#">Link Two</a>
      <a class="dropdown-item" href="#">Link Three</a>
      <div class="dropdown-divider"></div>
      <a class="dropdown-item" href="#">Link Four</a>
    </div>
</div>
```

Button groups:
```html
<div class="btn-group">
    <button class="btn" type="button">Left</button>
    <button class="btn" type="button">Middle</button>
    <button class="btn" type="button">Right</button>
</div>
```

Button toolbar:
```html
<div class="btn-toolbar">
    <div class="btn-group mr-2">
        <button class="btn" type="button">1</button>
        <button class="btn" type="button">2</button>
        <button class="btn" type="button">3</button>
        <button class="btn" type="button">4</button>
    </div>
    <div class="btn-group mr-2">
        <button class="btn" type="button">5</button>
        <button class="btn" type="button">6</button>
        <button class="btn" type="button">7</button>
    </div>
    <div class="btn-group">
        <button class="btn" type="button">8</button>
    </div>
</div>
```

Vertical button groups:
```html
<div class="btn-group-vertical">
    <button class="btn" type="button">Left</button>
    <button class="btn" type="button">Middle</button>
    <button class="btn" type="button">Right</button>
</div>
```

### _16. Navabars & Navs_

Simple navbar:
```html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
          <ul class="navbar-nav">
              <li class="nav-item">
                  <a class="nav-link" href="#">Home</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Contact</a>
              </li>
          </ul>
      </div>
</nav>
```
_Explanation of classes_:  
* _bg-light_: Can be swapped out for any bootstrap colors, like _bg-primary_, _bg-danger_, and _bg-success_.
* _navbar-light_: Should correspond to the background. _navbar-light_ will make your text readable on a light background, and _navbar-dark_ will make your text readable on a dark background.
* _navbar-brand_: The name of the website or page, separate from clickable nav items
* _navbar-expand-sm_: When the screen width hits the sm (small) mark, the nav items responsively lose their inline properties and become a vertical list to save space.

But what if you don't want a vertical list? What about a responsive toggle?
```html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler"
      data-toggle="collapse"
      data-target="#navbarNav"><span
      class="navbar-toggler-icon"></span></button>
          <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ml-auto">
              <li class="nav-item">
                  <a class="nav-link" href="#">Home</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Contact</a>
              </li>
          </ul>
        </div>
      </div>
</nav>
```

Navbar with form (and responsive toggle):
```html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler"
      data-toggle="collapse"
      data-target="#navbarNav"><span
      class="navbar-toggler-icon"></span></button>
          <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav mr-auto">
              <li class="nav-item">
                  <a class="nav-link" href="#">Home</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Contact</a>
              </li>
          </ul>

          <form class="form-inline my-2 my-lg-0">
            <input  type="text" class="form-control mr-sm-2"
            placeholder="Search">
            <button class="btn btn-outline-success my-2 my-sm-0">Search</button>
          </form>
        </div>
      </div>
</nav>
```

Navbar with dropdown:
```html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
          <ul class="navbar-nav">
              <li class="nav-item">
                  <a class="nav-link" href="#">Home</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle" data-toggle="dropdown">Dropdown</a>
                <div class="dropdown-menu">
                  <a href="#" class="dropdown-item">Link 1</a>
                  <a href="#" class="dropdown-item">Link 2</a>
                  <a href="#" class="dropdown-item">Link 3</a>
                </div>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Contact</a>
              </li>
          </ul>
      </div>
</nav>
```

Navs (essentially navbars with no background):
```html
<ul class="nav">
    <li class="nav-item">
        <a class="nav-link" href="#">Link 1</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 2</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 3</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 4</a>
    </li>
</ul>
```

Highlight active elements with _nav-pills_:
```html
<ul class="nav nav-pills">
    <li class="nav-item">
        <a class="nav-link active" href="#">Link 1</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 2</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 3</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 4</a>
    </li>
</ul>
```

_<ul>_ positioning classes for navs:
* _justify-content-center_: Center align
* _justify-content-end_: Right align
* _flex-column_: A column
* _nav-fill_: Makes the nav a block and gives each object an equal fill

Nav with dropdown:
```html
<ul class="nav nav-fill">
    <li class="nav-item">
        <a class="nav-link" href="#">Link 1</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 2</a>
    </li>
    <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle"
        href="#" data-toggle="dropdown">Dropdown</a>
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#">Link 1</a>
          <a class="dropdown-item" href="#">Link 2</a>
          <a class="dropdown-item" href="#">Link 3</a>
        </div>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 3</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 4</a>
    </li>
</ul>
```