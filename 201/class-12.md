# HTML canvas Element & Chart.js

## HTML canvas Element
The <canvas> element creates a fixed-size drawing surface.  It has only two attributes: `width` and `height`

> To display something, a script first needs to access the rendering context and draw on it. 

The <canvas> element has a method called getContext(), which takes one parameter; "2d" for 2D graphics.

#### Drawing shapes in canvas
Canvas has a grid (coordinate space) whith origin (0,0) at the top left corner.

Canvas has two primitive shapes (draw other shapes by using combining paths):
- rectangles
- paths

###### Rectangles
- fillRect(x, y, width, height) -filled rectangle
- strokeRect(x, y, width, height) -rectangular outline
- clearRect(x, y, width, height) - makes the area fully transparent

###### Paths
A path is a list of connected points. Make shapes using paths by:
- create the path: `beginPath()`, [path methods](https://developer.mozilla.org/en-US/docs/Web/API/CanvasRenderingContext2D#paths)
- draw into the path: `moveTo(x, y)`, `lineTo(x, y)`
- stroke or fill the path to render it: `stroke()`, `fill()`, `closePath()`
  - fillStyle = color, or strokeStyle = color
  - lineWidth = value, lineCap = type, etc.
  - createPattern(image, type)
    - repeat
    - repeat-x or repeat-y
    - no-repeat


***x and y refer to the top left corner of the shape***


---

## Chart.js
Chart.js is a JavaScript plugin that makes it realatively easy to draws graphs in <canvas>:
- Line
- Bar
- Radar
- Doughnut and Pie
- Polar Area
- Bubble
- Scatter
- Area
- Mixed types

To draw a graph use `new Chart(context, configuration` 
- context -canvas element.`getContext('2d')`
- configuaration -object containing `type`, `data` and `options`

---

[Back to table of contents](../README.md)