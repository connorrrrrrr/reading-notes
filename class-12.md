## Charts

- charts are better for displaying data visually than table.
- To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart.
```html
<canvas id="buyers" width="600" height="400"></canvas>
```
- Next a script that will retrieve the context of the canvas:
```html
<script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>
```
- inside the same script tags we need to create our data. This goes above the line that begins 'var buyers'.
##### Drawing a Pie Chart

```html
<canvas id="countries" width="600" height="400"></canvas>
```
- next the context and to instantiate the chart:
```javascript
var countries= document.getElementById("countries").getContext("2d");
new Chart(countries).Pie(pieData, pieOptions);
```
- next to create the data:
```javascript
var pieData = [
	{
		value: 20,
		color:"#878BB6"
	},
	{
		value : 40,
		color : "#4ACAB4"
	},
	{
		value : 10,
		color : "#FF8153"
	},
	{
		value : 30,
		color : "#FFEA88"
	}
  ```
##### Drawing a Bar Chart

```html
<canvas id="income" width="600" height="400"></canvas>
```
- next, retrieve the element and create the graph:
```javascript
var income = document.getElementById("income").getContext("2d");
new Chart(income).Bar(barData);
```
- now the bar chart's data:
```javascript
var barData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "#48A497",
			strokeColor : "#48A4D1",
			data : [456,479,324,569,702,600]
		},
		{
			fillColor : "rgba(73,188,170,0.4)",
			strokeColor : "rgba(72,174,209,0.4)",
			data : [364,504,605,400,345,320]
		}

	]
}
```
- the `<canvas>` element has two attributes, width and height.
- it creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.
#### Drawing
- `fillRect(x, y, width, height)` draws a filled rectangle
- `strokeRect(x, y, width, height)` draws a rectangular outline
- `clearRect(x, y, width, height)` clears the specified rectangular area, making it fully transparent.
- to draw a path, you create the path then use drawing commands to draw into it.
- `beginPath()` creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
- `closePath()` adds a straight line to the path, going to the start of the current sub-path.
- `stroke()` draws the shape by stroking its outline.
- `fill()` draws a solid shape by filling the path's content area.
- `moveTo(x, y)` moves the pen to the coordinates specified by x and y.
- for drawing straight lines, use the `lineTo()` method.
- to draw arcs or circles, use the `arc()` or `arcTo()` methods.
#### Colors
- `fillStyle = color`
  - this sets the style used when filling shapes.
- `strokeStyle = color`
  - this sets the style for shapes' outlines.
- `globalAlpha = transparencyValue`
  - applies the specified transparency value to all future shapes drawn on the canvas.
- `createPattern(image, type)`
  - creates and returns a new canvas pattern object.
  - the type specifies how to use the image in order to create the pattern, and must be one of the following string values:
  - `repeat` tiles the image in both vertical and horizontal directions.
  - `repeat-x` tiles the image horizontally but not vetically.
  - `repeat-y` tiles the image vertically but not horizontally.
  - `no-repeat` doesn't tile the image. It's only used once.
#### Drawing Text
- `fillText(text, x, y [, maxWidth])`
  - fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- `strokeText(text, x, y [, maxWidth])`
  - strokes a given text at the given (x,y) position. Optionally with a maximum width to draw. Ex:
  ```javascript
  function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.fillText('Hello world', 10, 50);
}
```

[<===Home](README.md)