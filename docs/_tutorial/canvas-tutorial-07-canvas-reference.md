---
title: Canvas Reference
---

# Canvas Reference

[Xiao Shang](http://ishx.io) 

## Description

The HTML5 `<canvas>` tag is used to draw graphics, on the fly, via scripting (usually JavaScript).

However, the `<canvas>` element has no drawing abilities of its own (it is only a container for graphics) - you must use a script to actually draw the graphics.

The `getContext()` method returns an object that provides methods and properties for drawing on the canvas.

This reference will cover the properties and methods of the `getContext("2d")` object, which can be used to draw text, lines, boxes, circles, and more - on the canvas.

## Browser Support

The numbers in the table specify the first browser version that fully supports the element.

Element | ![alt-text][chrome] | ![alt-text][edge] | ![alt-text][firefox] | ![alt-text][safari] | ![alt-text][opera]
 --- | --- | --- | --- | --- | ---
`<canvas>` | 4.0 | 3.0 | 2.0 | 3.1 | 9.0

[chrome]: assets/img/compatible_chrome.gif "Chrome"

[edge]: assets/img/compatible_edge.gif "Edge"

[firefox]: assets/img/compatible_firefox.gif "Firefox"

[safari]: assets/img/compatible_safari.gif "Safari"

[opera]: assets/img/compatible_opera.gif "Opera"

Internet Explorer 9, Firefox, Opera, Chrome, and Safari support `<canvas>` and its properties and methods.

**Note:** Internet Explorer 8 and earlier versions, do not support the `<canvas>` element.

## Colors, Styles, and Shadows

Property | Description
 --- | --- 
fillStyle | Sets or returns the color, gradient, or pattern used to fill the drawing
strokeStyle	| Sets or returns the color, gradient, or pattern used for strokes
shadowColor	| Sets or returns the color to use for shadows
shadowBlur	| Sets or returns the blur level for shadows
shadowOffsetX | Sets or returns the horizontal distance of the shadow from the shape
shadowOffsetY | Sets or returns the vertical distance of the shadow from the shape

Method | Description
 --- | ---
createLinearGradient() | Creates a linear gradient (to use on canvas content)
createPattern() | Repeats a specified element in the specified direction
createRadialGradient() | Creates a radial/circular gradient (to use on canvas content)
addColorStop() | Specifies the colors and stop positions in a gradient object

## Line Styles

Property | Description
 --- | ---
lineCap | Sets or returns the style of the end caps for a line
lineJoin | Sets or returns the type of corner created, when two lines meet
lineWidth | Sets or returns the current line width
miterLimit | Sets or returns the maximum miter length

## Rectangles

Method | Description
 --- | ---
rect() | Creates a rectangle
fillRect() | Draws a "filled" rectangle
strokeRect() | Draws a rectangle (no fill)
clearRect() | Clears the specified pixels within a given rectangle

# Paths

Method | Description
 --- | ---
fill() | Fills the current drawing (path)
stroke() | Actually draws the path you have defined
beginPath() | Begins a path, or resets the current path
moveTo() | Moves the path to the specified point in the canvas, without creating a line
closePath() | Creates a path from the current point back to the starting point
lineTo() | Adds a new point and creates a line to that point from the last specified point in the canvas
clip() | Clips a region of any shape and size from the original canvas
quadraticCurveTo() | Creates a quadratic Bézier curve
bezierCurveTo() | Creates a cubic Bézier curve
arc() | Creates an arc/curve (used to create circles, or parts of circles)
arcTo() | Creates an arc/curve between two tangents
isPointInPath() | Returns true if the specified point is in the current path, otherwise false

## Transformations

Method | Description
 --- | ---
scale() | Scales the current drawing bigger or smaller
rotate() | Rotates the current drawing
translate() | Remaps the (0,0) position on the canvas
transform() | Replaces the current transformation matrix for the drawing
setTransform() | Resets the current transform to the identity matrix. Then runs transform()

# Text

Property | Description
 --- | ---
font | Sets or returns the current font properties for text content
textAlign | Sets or returns the current alignment for text content
textBaseline | Sets or returns the current text baseline used when drawing text

Method | Description
 --- | ---
fillText() | Draws "filled" text on the canvas
strokeText() | Draws text on the canvas (no fill)
measureText() | Returns an object that contains the width of the specified text

## Image Drawing

Method | Description
 --- | ---
drawImage() | Draws an image, canvas, or video onto the canvas

# Pixel Manipulation

Property | Description
 --- | ---
width | Returns the width of an ImageData object
height | Returns the height of an ImageData object
data | Returns an object that contains image data of a specified ImageData object

Method | Description
 --- | ---
createImageData() | Creates a new, blank ImageData object
getImageData() | Returns an ImageData object that copies the pixel data for the specified rectangle on a canvas
putImageData() | Puts the image data (from a specified ImageData object) back onto the canvas

## Compositing

Property | Description
 --- | ---
globalAlpha | Sets or returns the current alpha or transparency value of the drawing
globalCompositeOperation | Sets or returns how a new image are drawn onto an existing image

## Other

Method | Description
 --- | ---
save() | Saves the state of the current context
restore() | Returns previously saved path state and attributes
createEvent() | 
getContext() | 
toDataURL() |
