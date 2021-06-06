# Charts:
Are a better way for dispalying data visually than tables. Where it provides features to make your data look cool and presentable and it can convey data quickly but they are not easy to create. 
JS plugin Uses HTML5 canvas to allow you to draw a graph on the page, Those plugin are well documented that makes all kind of **Bar charts**, **Line Charts**, and **Pie Charts** increadibly easy to use. Before using them we nned to download charts.

## Drawing Line Chart:
1. First we need to create a canvas element in our HTML file
2. we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element.
3. Create our data 

## Drawing Pie Chart:
1. Just like the line chart we need a canvas element 
2. Then we are going to need to get a context to instantiate the chart.
3. we need to create the data. This data is a little different to the line chart because the pie chart is simpler,we just need to supply a value and a color for each section.
4. We need to add our options which are two things:
  1. We need to remove the stroke from the segments.
  2. Then we animate the scale of the pie so that it zoom out from nothing.

## Drawing a Bar Chart:
1. As we did in our pie and inline charts we need the same syntax which is the canvas.
2. Then we need to retrive the element and create a graph.
3. Then we add the data for our bar chart.

# Canvas API:
As we disscussed before when we want to create any chart we need **Canvas Element**. What is canvas??
Canvas is similar to img tag in HTML where the only clear difference is that canvas doesnt use src and alt attributes where it uses width or height but even width and height are optional in canvas. If we do not specify a value for the width and height then it will be the default value that is **300 Pixels Width** and **150 Pixels Height**. Canvas is like any element out there in HTML that can be edited in CSS.
**VIP** if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.

The id attribute isn't specific to the canvas element but is one of the global HTML attributes which can be applied to any HTML element (like class for instance). It is always a good idea to supply an id because this makes it much easier to identify it in a script.

The canvas element can be styled just like any normal image (margin, border, background…). These rules, however, don't affect the actual drawing on the canvas. We will see how this is done in a dedicated chapter of this tutorial. When no styling rules are applied to the canvas it will initially be fully transparent.

## FallBack Content:
Canvas is similar to the audio tag, video tag, and picture tag where it can easily define some fallback content, to be displayed in older browsers not supporting it, for instance: versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

## How to provide Fallback Content???
We just need to insert the alternate content inside the canvas element. Browsers that don't support canvas will ignore the container and render the fallback content inside it. Browsers that do support canvas will ignore the content inside the container, and just render the canvas normally.

## Does the canvas element requires a closing tag??
Yes it **requires** it unlike the img tag that does not have a closing tag.

## Drawing Shapes with Canvas:
We can shapes using canvas such as rectangles, triangles, lines, arcs and curves. First we will start with:
1. Drawing rectangles: Unlike SVG, canvas only supports two primitive shapes: rectangles and paths All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes. There are three functions in in canvas that helps us to design rectangle: 
  1. fillRect(x, y, width, height): Draws a filled rectangle.
  2. strokeRect(x, y, width, height): Draws a rectangular outline.
  3. clearRect(x, y, width, height): Clears the specified rectangular area, making it fully transparent.

2. Drawing paths:
A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:
 1. First, you create the path.
 2. Then you use drawing commands to draw into the path..
 3. Once the path has been created, you can stroke or fill the path to render it.
below are some of the functions that are used to perform the above steps:
 1. beginPath()
 2. Path methods
 3. closePath()
 4. stroke()
 5. fill()

MoveTo(x, y) function: Moves the pen to the coordinates specified by x and y. We could also use moveTo() to draw unconnected paths.

LinesTo(x, y) function: Draws a line from the current drawing position to the position specified by x and y.For drawing straight lines, the starting point is dependent on previously drawn paths, where the end point of the previous path is the starting point for the following.  The starting point can also be changed by using the moveTo() method. 

arc(x, y, radius, startAngle, endAngle, counterclockwise): Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by counterclockwise (defaulting to clockwise).
arcTo(x1, y1, x2, y2, radius): Draws an arc with the given control points and radius, connected to the previous point by a straight line.   

# Applying Styles and Colors:
There are two important properties that can be used for colors:
1. fillStyle = color: Sets the style used when filling shapes.
2. strokeStyle = color: Sets the style for shapes' outlines.    

Transparency: It uses the globalAlpha property by assigning a semi transparent color to the stroke and/or fill style. GlobalAlpha property can be useful if you want to draw a lot of shapes on the canvas with similar transparency, but otherwise it's generally more useful to set the transparency on individual shapes when setting their colors.

Line Styles: We have several properties which allows us to style line:
1. lineWidth = value: Sets the width of lines drawn in the future.
2. lineCap = type: Sets the appearance of the ends of lines.
3. lineJoin = type: Sets the appearance of the "corners" where lines meet.
4. miterLimit = value: Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
5. getLineDash(): Returns the current line dash pattern array containing an even number of non-negative numbers.
6. setLineDash(segments): Sets the current line dash pattern.
7. lineDashOffset = value: Specifies where to start a dash array on a line.