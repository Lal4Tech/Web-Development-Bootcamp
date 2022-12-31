# Bootstrap

## Introduction

**Front-End**
Languages:

- HTML
- CSS
- Javascript

**back-End**
Languages:

- .NET
- Ruby
- PHP
- Java
- NodeJS
- SQL

**Bootstrap** is on the front-end. It's a bunch of code that was written to be reusable and make designing website much easier.

**Responsive** means that how it responds to the viewport. That means website become adaptive, your website changes its design depending on where it's  being displayed. Bootstrap makes it very easier.

## Bootstrap

[Official Introduction](https://getbootstrap.com/docs/5.2/getting-started/introduction/)

### Installation

1. Link cdn url for Bootstrap css/js in html head.
2. Use bootstrap boiler plate code from official website.
3. Download from official website and include it in the website source directory.

## Wireframing

- Low fidelity representation and less time consuming.
- Contrary to mock-up which is a high fidelity representation of your design.
- [UI-Patterns.com](https://ui-patterns.com/)
- [Dribbble](https://dribbble.com/)
- For Wireframing 
  - [Sneakpeekit](https://sneakpeekit.com/)
  - Industry standard tool [Balsamiq](https://balsamiq.com/)
  
## Bootstrap Navigation Bar

- [Navbar doc](https://getbootstrap.com/docs/5.2/components/navbar/)
- [Background](https://getbootstrap.com/docs/5.2/utilities/background/)
- [Spacing](https://getbootstrap.com/docs/5.2/utilities/spacing/)
- [Toggler](https://getbootstrap.com/docs/5.2/components/navbar/#toggler)

```css
<nav class="navbar navbar-expand-lg navbar-light bg-dark">
    <a class="navbar-brand" href="">tindog</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
    <ul class="navbar-nav ms-auto">
        <li class="nav-item">
            <a class="nav-link" href="">Contact</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Pricing</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Download</a>
        </li>
    </ul>
    </div>
</nav>
```

## Bootstrap Grid Layout System

Doc: [Grid Layout](https://getbootstrap.com/docs/5.2/layout/grid/)

```html
<!-- 2 columns each taking 50% of width -->
<div class="row">
    <div class="col" style="background-color: red; border: 1px solid;">
        col
    </div>
    <div class="col" style="background-color: red; border: 1px solid;">
        col
    </div>
</div>
```

There are 12 template columns available per row

```html
<!-- Each column is taking 6 units(out of 12). But non-responsive -->
<div class="row">
    <div class="col-6" style="background-color: green; border: 1px solid;">
        col-6
    </div>
    <div class="col-6" style="background-color: green; border: 1px solid;">
        col-3
    </div>
</div>
```

To make it responsive to view ports:

```html
<!-- Each column is taking 6 units(out of 12) for vew port size from medium size. -->
<div class="row">
    <div class="col-md-6" style="background-color: yellow; border: 1px solid;">
        col-md-6
    </div>
    <div class="col-md-6" style="background-color: yellow; border: 1px solid;">
        col-md-6
    </div>
</div>
```

**col-md-6** means that we should have 6 unit column on any view port size from medium/tablet size or upwards. But for anything smaller than that, such as on mobile phone, they will take up the full width.

**col-lg-3** means anything smaller(tablet/mobile) than desktop, column will take 100% of width.

```html
<div class="row">
    <div class="col-lg-3" style="background-color: yellow; border: 1px solid;">
        col-lg-3
    </div>
    <div class="col-lg-3" style="background-color: yellow; border: 1px solid;">
        col-lg-3
    </div>
    <div class="col-lg-3" style="background-color: yellow; border: 1px solid;">
        col-lg-3
    </div>
    <div class="col-lg-3" style="background-color: yellow; border: 1px solid;">
        col-lg-3
    </div>
</div>
```

**col-lg-3 col-md-4 col-sm-6**: Column take quarter of width when we are on desktop or larger, but only one third of width  when we are on tablet, and only half of the width when we are on mobile.

```html
<div class="row">
    <div class="col-lg-3 col-md-4 col-sm-6" style="background-color: yellow; border: 1px solid;">
        col-lg-3 col-md-4 col-sm-6
    </div>
    <div class="col-lg-3 col-md-4 col-sm-6" style="background-color: yellow; border: 1px solid;">
        col-lg-3 col-md-4 col-sm-6
    </div>
    <div class="col-lg-3 col-md-4 col-sm-6" style="background-color: yellow; border: 1px solid;">
        col-lg-3 col-md-4 col-sm-6
    </div>
    <div class="col-lg-3 col-md-4 col-sm-6" style="background-color: yellow; border: 1px solid;">
        col-lg-3 col-md-4 col-sm-6
    </div>
</div>
```
