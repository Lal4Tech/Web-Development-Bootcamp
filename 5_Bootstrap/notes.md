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

