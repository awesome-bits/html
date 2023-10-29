# Scripting

To create dynamic content and Web applications, HTML supports the use of scripting languages, most prominently JavaScript. Certain elements support this capability.

## Script

The `<script>` element either contains scripting statements, or it points to an external script file through the src attribute.

```html
<div id="demo"></div>
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
```

```html
<script src="myscript.js"></script>
```

## Noscript

The `<noscript>` element defines an alternate content for users that have disabled scripts in their browser or have a browser that doesn't support script.

```html
<noscript>Your browser does not support JavaScript!</noscript>
```

## Canvas

The canvas element is used to draw graphics, on the fly, via scripting (usually JavaScript). However, the `<canvas>` element has no drawing abilities of its own (it is only a container for graphics) - you must use a script to actually draw the graphics.

Canvas has several methods for drawing paths, boxes, circles, text, and adding images.

```html
<canvas id="myCanvas" width="200" height="100" style="border:1px solid #000000;">
</canvas>
<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  ctx.fillStyle = "#FF0000";
  ctx.fillRect(0,0,150,75);
</script>
```
