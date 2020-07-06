---
layout: post
title: 'Test post for hosting D3.js visualizations'
tags: [JavaScript, Tips, D3.js]
featured_image_thumbnail:
featured_image:
featured: true
hidden: true
jsarr:
     - graphs/barchart_test.js
---

> "Quotes are nice, but most are made up." <cite>- Somebody, probably -</cite>


## My effort to embed a custom D3.js viz

> this is a blockquote

<div id="chart"></div>
<p id="clicktest">Click me, please!</p>

<script src="https://d3js.org/d3.v5.js"></script>
<script>
data = [20, 30, 40, 22, 13, 7, 42, 27];

var w =  800;
var h = 400;
var margin = ({top: 20, right: 30, bottom: 30, left: 40});

var y = d3.scaleLinear()
     .domain([0, d3.max(data)])
     .range([h - margin.bottom, margin.top]);

var x = d3.scaleBand()
     .domain(d3.range(data.length))
     .rangeRound([margin.left, w - margin.right])
     .padding(0.1);

var svg = d3.select('#chart')
     .classed("svg-container", true)
     .append('svg')
     .attr("preserveAspectRatio", "xMinYMin meet")
     .attr("viewBox", "0 0 600 400")
     .classed("svg-content-responsive", true)
     .attr('width', w )
     .attr('height', h );
   
yTitle = g => g.append('text')
     .attr('font-family', 'sans-serif')
     .attr('y', 13)
     .attr('x', 2)
     .text('↑ Value');

yAxis = g => g
     .attr('transform', 'translate(' + margin.left + ')')
     .call(d3.axisLeft(y).tickSizeOuter(0)) //.ticks(null, "%"))
     .call(g => g.select(".domain")) //.remove()); This is how you remove main line

xAxis = g => g
     .attr('transform', 'translate(0,' + (h - margin.bottom) + ')')
     .call(d3.axisBottom(x).tickSizeOuter(0));

var bar = svg.selectAll('rect')
     .data(data)
     .enter()
     .append('rect')
     .attr('x', (d, i) => x(i) )
     .attr('y', d => y(d))
     .attr('width', x.bandwidth())
     .attr('height', d => y(0) - y(d))
     .attr('fill', 'steelblue');

svg.append('g')
     .call(xAxis);

svg.append('g')
     .call(yAxis);

svg.append('g')
     .call(yTitle);


svg.append('g')
   .selectAll('text')
   .text(function(d) {
     return d;
   })
   .attr('x', (d, i) => x(i) + x.bandwidth() / 2)
   .attr('y', (d) => h - y(d));

d3.select('#clicktest')
  .on('click', function() {

    var dataset = data.sort(d3.ascending);

    svg.selectAll('rect')
       .data(dataset)
       .transition()
       .delay(function(d, i) {
         return i * 50;
       })
       .attr('x', (d, i) => x(i))
       .attr('y', d => y(d))
       .attr('width', x.bandwidth())
       .attr('height', d => y(0) - y(d));
  });
    
</script>

<style>
.svg-container {
  display: inline-block;
  position: relative;
  width: 80%;
  padding-bottom: 80%; /* aspect ratio */
  vertical-align: top;
  overflow: hidden;
}
.svg-content-responsive {
  display: inline-block;
  position: absolute;
  top: 10px;
  left: 0;
}
</style>