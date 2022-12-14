Javascript Canvas

  Canvas allows you to try 2D images using JS. It requires the attributes height and width to so that the size of the canvas is specified.

  It is important to always close the canvas tag ( ex. </canvas>) beause any content between the opening and closing tags is considered fallback content and it will only be displayed if the browser doesn't support the canvas element.

  getContext() is a method featured in the canvas element. Its purpose  is to return a render context object.

    Example - Selecting the canvas element using the querySelector() method and accessing the canvas by calling its getContext() method:

      let canvas = document.querySelector('#canvas);
      let ctx = main.getContext('2d');

Chart.js

    "Chart.js is highly customizable with custom plugins to create annotations, zoom, or drag-and-drop functionalities to name a few things."

    "Chart.js comes with a sound default configuration, making it very easy to start with and get an app that is ready for production. Chances are you will get a very appealing chart even if you don’t specify any options at all. For instance, Chart.js has animations turned on by default, so you can instantly bring attention to the story you’re telling with the data."

    3 Chart Types created by Chart.js

    - Area Chart
    - Doughnut and Pie Charts
    - Bubble Chart

  Chart data is easier to view and read quickly but it's harder to create. 
  Chart.js could aid previously created applications by presenting the data from polls taken, such as in the Odd Duck Lab from yesterday, and presenting it in a chart that makes it easier to quickly read

Source:

  https://www.javascripttutorial.net/web-apis/javascript-canvas/
  https://www.chartjs.org/docs/latest/
  https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/
