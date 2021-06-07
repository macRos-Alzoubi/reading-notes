# Chart.js, Canvas

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

## Setting up

  The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in.

  - ### Installation

    You can get the latest version of Chart.js from [npm](https://www.npmjs.com/package/chart.js) , the [GitHub releases](https://github.com/chartjs/Chart.js/releases/tag/v3.3.2) , or use a [Chart.js CDN](https://www.jsdelivr.com/package/npm/chart.js). Detailed installation instructions can be found on the [installation](https://www.chartjs.org/docs/latest/getting-started/installation.html) page.
  
  Then create a new html page and import the script:

  ```html
  
  <!DOCTYPE html>
  <html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <script src='Chart.min.js'></script>
    </head>
    <body>
    </body>
  </html>
  ```

## Drawing a line chart

  To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:

  ```html
  <canvas id="buyers" width="600" height="400"></canvas>
  ```

  Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:

  ```js
  <script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
  </script>
  ```

  Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart. Add this immediately above the line that begins `var buyers=`:

  ```js
  var buyerData = {
   labels : ["January","February","March","April","May","June"],
   datasets : [
    {
     fillColor : "rgba(172,194,132,0.4)",
     strokeColor : "#ACC26D",
     pointColor : "#fff",
     pointStrokeColor : "#9DB86D",
     data : [203,156,99,251,305,247]
   }
  ]
 }
  ```

## Drawing a pie chart

   First, we need the canvas element:

 ```html
 <canvas id="countries" width="600" height="400"></canvas>
 ```

 Next, we need to get the context and to instantiate the chart:

 ```js
 var countries= document.getElementById("countries").getContext("2d");
 new Chart(countries).Pie(pieData, pieOptions);
 ```

 Next we need to create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each section:

 ```js
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
];
 ```

 Now, immediately after the pieData we’ll add our options:

 ```js
 var pieOptions = {
 segmentShowStroke : false,
 animateScale : true
}
 ```

 These options do two things, first they remove the stroke from the segments, and then they animate the scale of the pie so that it zooms out from nothing.

## Drawing a bar chart

  First, we add the canvas element, As in Pi Chart and Line Chart:

  ```html
  <canvas id="income" width="600" height="400"></canvas>
  ```

  Next, we retrieve the element and create the graph:

  ```js
  var income = document.getElementById("income").getContext("2d");
  new Chart(income).Bar(barData);
  ```

  And finally, we add in the bar chart’s data:

  ```js
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

  The great things about Chart.js are that it’s simple to use and really very flexible. Plus, once you’ve mastered the basics here, you’ll discover that there are tons of options listed in the documentation.
