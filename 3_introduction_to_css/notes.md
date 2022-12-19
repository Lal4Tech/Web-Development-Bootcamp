## Inline css
```
<body style="background-color: blue;"></body>
```

## Internal css
```
<head>
    <style>
        body {
            background-color: #CFF5E7;
        }
    </style>
</head>
```

## External css
```
<head>
    <link rel="stylesheet" type="text/css" href="css/styles.css">
</head>
```

## CSS preferences
Inline >> Internal >> External 

## Default CSS applied by the browser
For some elements browsers apply some default css properties. We have to overwrite to change those parameters.

## CSS syntax
```
selector {
    property: value;
}
```
*selector ::: who*
*property ::: what*
*value ::: how*

## CSS selectors
Preference: ID selector > Tag selector
id should be unique. But class can be used to group multiple elements(same class value for multiple elements possible)
### TAG selectors
```
body {
    background-color: rgb(135, 154, 206);
}

h1 {
    color: rgb(30, 11, 122);
    font-size: 100px;
}

img {
    background-color: red;
}
```

### CLASS selectors
```
.bacon {
    background-color: green;
}

.eggplant {
    background-color: red;
}
```

### ID selectors
```
#heading {
    color: blue;
}
```

**Notes**:
- multiple classes for one element possible
- But multiple ids for one element is not possible

## Pseudo classes
```
img:hover {
    background-color: gold;
}
```