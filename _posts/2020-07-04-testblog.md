---
layout: post
title: 'Test post for hosting D3.js visualizations'
tags: [JavaScript, Tips, D3.js]
featured_image_thumbnail:
featured_image:
featured: true
hidden: true
---

> "Quotes are nice, but most are made up." <cite>- Somebody, probably -</cite>


## My effort to embed a custom D3.js viz

> this is a blockquote

<div id="div_basicResize"></div>

<script src="https://d3js.org/d3.v4.js"></script>

<script>

var Svg = d3.select("#div_basicResize")
  .append("svg")
  .attr("height", 200);

var data = [19, 13, 54, 78, 98, 120, 138];

var x = d3.scaleLinear()
  .domain([0, 150]);
    
var xAxis = Svg.append("g")
  .attr("transform", "translate(0,150)");

var myCircles = Svg
  .selectAll("circles")
  .data(data)
  .enter()
  .append("circle")
    .style("fill", "#69b2b3")
    .attr("r", 20)
    .attr("cy", 100);

function drawChart() {

  // get the current width of the div where the chart appear, and attribute it to Svg
  currentWidth = parseInt(d3.select('#div_basicResize').style('width'), 10)
  Svg.attr("width", currentWidth)

  // Update the X scale and Axis (here the 20 is just to have a bit of margin)
  x.range([ 20, currentWidth-20 ]);
  xAxis.call(d3.axisBottom(x))

  // Add the last information needed for the circles: their X position
  myCircles
    .attr("cx", function(d){ return x(d)})
  };


// Initialize the chart
drawChart();

// Add an event listener that run the function when dimension change
window.addEventListener('resize', drawChart );


</script>