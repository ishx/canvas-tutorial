---
title: Canvas Text
---

# Canvas Text

[Xiao Shang](http://ishx.io) 

## Drawing Text on the Canvas

To draw text on a canvas, the most important property and methods are:

- font - defines the font properties for the text
- fillText(text,x,y) - draws "filled" text on the canvas
- strokeText(text,x,y) - draws text on the canvas (no fill)

## Using fillText()

Set font to 30px "Arial" and write a filled text on the canvas:

JavaScript:

```
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.font = "30px Arial";
ctx.fillText("Hello World",10,50);
```

## Using strokeText()

Set font to 30px "Arial" and write a text, with no fill, on the canvas:

JavaScript:

```
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.font = "30px Arial";
ctx.strokeText("Hello World",10,50);
```

# Add Color and Center Text

Set font to 30px "Comic Sans MS" and write a filled red text in the center of the canvas:

JavaScript:

```
var canvas = document.getElementById("myCanvas");
var ctx = canvas.getContext("2d");
ctx.font = "30px Comic Sans MS";
ctx.fillStyle = "red";
ctx.textAlign = "center";
ctx.fillText("Hello World", canvas.width/2, canvas.height/2);
```
