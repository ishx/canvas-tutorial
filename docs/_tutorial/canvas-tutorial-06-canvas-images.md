---
title: Canvas Images
---

# Canvas Images

[Xiao Shang](http://ishx.io) 

To draw an image on a canvas, use the following method:

- `drawImage(image,x,y)`

JavaScript:

```
window.onload = function() {
    var canvas = document.getElementById("myCanvas");
    var ctx = canvas.getContext("2d");
    var img = document.getElementById("scream");
    ctx.drawImage(img, 10, 10);
};
```