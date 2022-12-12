# Intermediate CSS notes
## Add css file to page

```
<head>
    <title>Document</title>
    <link rel="stylesheet" href="css/styles.css">
    <link rel="icon" href="favicon.ico">
</head>
```

## favicon 
https://www.favicon.cc/

```
<head>
    <title>Document</title>
    <link rel="icon" href="favicon.ico">
</head>
```

## Box model
```
<body>
    <div class="top-container">
        <h1>I'm Lal</h1>
        <p>a programmer</p>
    </div>
    <div class="middle-container">

    </div>
    <div class="bottom-container">

    </div>
</body>
</html>
```

## CSS Display properties 
- Block
- Inline
- Inline-Block
- None

### Block

By default some elements are block display. eg: h1, p etc. They take whole width of the screen on a page.
eg: Paragraphs, headers, divisions, lists and list items, forms

### Inline
Inline display element(unlike block elements) only take the space it needs to.
eg: spans, images, anchors
We can't change width of elements
to make block elements inline, we can set its display property to inline 
same way we can make dsiplay property block for an inline element.

### Inline-block 
by using display property inline-block we can make elements in the same line and also will be able to change its width.


### None
----
Remove the elements from the website as if it doesn't exists.
But when you set property visibility to hidden, it consume the space but just hidden.


## CSS Static and relative positioning
Even without CSS html elements already have pre-defined rules on how they displayed on a webpage. The rules for this are: 
1. Content is everything
Content decide how much space an element take 

2. Order comes from Code 
```
<h1></h1>
<p></p>
<p></p>
<p></p>
<img>
```
Here image appear at the end.
But below it appears in the beginning.
```
<img>
<h1></h1>
<p></p>
<p></p>
<p></p>
```

3. Children Sit on top of Parents
```
<div>
    <h1>a programmer</h1>
</div>
```
Here heading sit on top of div. --> z-index 

### Position
Used in order to have custom position instead of going with default layout.

1. Static
All html elements are static in their default position. This is the position without any css. 

2. Relative
Position the element relative w.r.t how it would have been positioned had it been static.
```
img {
    position: relative;
    left: 30px;
}
```
here the image will be pushed 30px from the left of previous position.

coordinates specified by top, bottom, left, right

It doesn't affect position of anything else on the screen.

eg:
```
<body>
  <div class="red">
  </div>
  
  <div class="blue">
  </div>
  
  <div class="yellow">
  </div>
</body>

.red {
  height: 100px;
  width: 100px;
  background-color: red;
  position: relative;
  left: 200px;
  top: 200px;
}

.blue {
  height: 100px;
  width: 100px;
  background-color: blue;
  position: relative;
  left: 100px;
}

.yellow {
  height: 100px;
  width: 100px;
  background-color: yellow;
  position: relative;
  bottom: 200px;
}
```

In above, before applying css, the red, blue and yellow elements appear one after another from top to bottom. But after applying the yellow, blue, red from top to bottom but corner to corner w.r.t other.

3. Absolute
```
dif {
    position: relative;
}

img {
    position: absolute;
    left: 30px;
}
```
Positioning the child element relative to its parent. Here the image will be 30px from right of the div.

This can be used to make the element out of normal html flow.

If an element have its position set as absolute, in order to position it relative to something one of it's parents has to have its position set as relative.

eg:
```
<body>
  <div class="red">
  </div>
  
  <div class="blue">
  </div>
  
  <div class="yellow">
  </div>
</body>

body {
  margin: 0;
}

.red {
  height: 100px;
  width: 100px;
  background-color: red;
  position: absolute;
  left: 200px;
  top: 200px;
}

.blue {
  height: 100px;
  width: 100px;
  background-color: blue;
  position: absolute;
  left: 100px;
  top: 100px;
}

.yellow {
  height: 100px;
  width: 100px;
  background-color: yellow;
  position: absolute;
}
```
Same implementation mentioned in 'relative' positioning section, but here using absolute position.

4. Fixed

Used if we want to fix an element in the same position even during the scrolling. eg: nav bar. 

```
<body>
  <div class="container">
    <div class="red">
    </div>
  </div>
  
  <div class="blue">
  </div>
  
  <div class="yellow">
  </div>
  
  <h1>Hello World</h1>
  <h1>Hello World</h1>
  <h1>Hello World</h1>
  <h1>Hello World</h1>
  <h1>Hello World</h1>
  <h1>Hello World</h1>
  <h1>Hello World</h1>
  <h1>Hello World</h1>
  <h1>Hello World</h1>
  <h1>Hello World</h1>
</body>

body {
  margin: 0;
}

.container {
  position: relative;
  width: 300px;
  height: 300px;
  background-color: grey;
}

.red {
  height: 100px;
  width: 100px;
  background-color: red;
  position: absolute;
  left: 200px;
}

.blue {
  height: 100px;
  width: 100px;
  background-color: blue;
  position: absolute;
  left: 100px;
  top: 0;
}

.yellow {
  height: 100px;
  width: 100px;
  background-color: yellow;
  position: fixed;
  top: 0;
}
```

## Centering elements with CSS
*text-align: center* inside the container or the parent element will center everything inside that doesn't have a width set.
If it's a block element and it have a width set, then we can center it with auto value in the margin.
```
margin: 0 auto 0 auto;

<!.. can shorten this: top and bottom 0 and left and right auto>
margin: 0 auto;
```

## Font styling
There are two major font families:
- Serif
- Sans-Serif

Web safe CSS font stacks : https://www.cssfontstack.com/

eg: 
```font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;```
This means if the font Helvetica Neue is installed in the system it will be used, otherwise it will use second and so on.
So, going from specific to less specific based on availability.

### Font embedding
https://fonts.google.com/

```<link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Merriweather+Sans&family=Montserrat&family=Sacramento&display=swap" rel="stylesheet">```

If the user don't have this font already installed, browser take them to this location and grab those fonts. 