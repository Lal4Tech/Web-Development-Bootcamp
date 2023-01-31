# Intermediate Bootstrap

## Bootstrap Carousel

A slideshow component for cycling through elements—images or slides of text—like a carousel.
On this page

Official doc: [Carousel](https://getbootstrap.com/docs/5.2/components/carousel/)

eg: with control for slide

```html
<div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active" style="background-color: red;">
      <img src="..." class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item" style="background-color: yellow;">
      <img src="..." class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item" style="background-color: blue;">
      <img src="..." class="d-block w-100" alt="...">
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
```

```css
.carousel-item {
    height: 500px;
}
```

