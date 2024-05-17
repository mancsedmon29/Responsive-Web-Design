# Learn CSS Colors by Building a Set of Colored Markers

Making the right color choices for your website can significantly increase readers' visual attractiveness.

You will assemble a set of colorful markers during this session. You'll discover many techniques for assigning values to colors and for matching colors.

`index.html`

```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Colored Marker</title>
        <link rel="stylesheet" href="styles.css">
    </head>
    <body>
        <h1>CSS Color Markers</h1>
        <div class="container">
            <div class="marker red">
                <div class="cap"></div>
                <div class="sleeve"></div>
            </div>
            <div class="marker green">
                <div class="cap"></div>
                <div class="sleeve"></div>
            </div>
            <div class="marker blue">
                <div class="cap"></div>
                <div class="sleeve"></div>
            </div>
        </div>
    </body>
</html>
```

`style.css`

```
h1 {
    text-align: center;
}
  
.marker {
    height: 25px;
    width: 200px;
    margin: 10px auto;
}

.container {
    background-color: rgb(255, 255, 255);
    padding: 10px 0;
}

.red {
    background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
    box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8);
}

.green {
    background: linear-gradient(#55680D, #71f53e, #116c31);
    box-shadow: 0 0 20px 0 #3b7e20cc;
}

.blue {
    background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
    box-shadow: 0 0 20px 0 hsla(223, 59%, 31%, 0.8);
}

.sleeve {
    width: 110px;
    height: 25px;
    background-color: rgba(255, 255, 255, 0.5);
    border-left: 10px double rgba(0, 0, 0, 0.75);
}

.cap {
    width: 60px;
    height: 25px;
}

.cap, .sleeve {
    display: inline-block;
}
```
