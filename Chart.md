# Chart
Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

 great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

 ## how to Setting up

The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script:
 <script src='Chart.min.js'\></script\>

 2. Drawing a line chart
<canvas id="buyers" width="600" height="400"\></canvas\>

we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element

 var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
    Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart. Add this immediately above the line that begins ‘var buyers=’:
    3.Drawing a pie chart

Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element:
<canvas id="countries" width="600" height="400"></canvas>
Next, we need to get the context and to instantiate the chart:

var countries= document.getElementById("countries").getContext("2d");
new Chart(countries).Pie(pieData, pieOptions);

Drawing a bar chart

<canvas id="income" width="600" height="400"></canvas>

Next, we retrieve the element and create the graph:

var income = document.getElementById("income").getContext("2d");
new Chart(income).Bar(barData);
And finally, we add in the bar chart’s data

### Basic usage of canvas
Let's start this tutorial by looking at the <canvas> HTML element itself. At the end of this page, you will know how to set up a canvas 2D context and have drawn a first example in your browser.
The <\canvas> element

Drawing shapes with canvas
Now that we have set up our canvas environment, we can get into the details of how to draw on the canvas. By the end of this article, you will have learned how to draw rectangles, triangles, lines, arcs and curves, providing familiarity with some of the basic shapes. Working with paths is essential when drawing objects onto the canvas and we will see how that can be done.



