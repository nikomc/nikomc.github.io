---
layout: post
title:  "Dynamically Updating Bar Chart - D3.js"
tags: [ D3, D3.js, dataviz ]
featured_image_thumbnail:
featured_image:
featured:
hidden:

---

I have studied data visualization every day for the last three months, in an effort to improve my skills, but progress has been slow. The learning curve is steep.

In learning D3.js, I've tried most resources: YouTube videos, Udemy courses, and a range of books. The best book that I've encountered for learning D3.js is Scott Murray's _Interactive Data Visualization for the Web_, which provides a solid foundation and assumes little prior knowledge. In Chapter 9, Murray builds a bar chart that updates dynamically when the user clicks on a paragraph element -- a new bar comes in when the user clicks on text reading "Add a bar", and a bar slides out when the user clicks on text reading "Remove a bar". It's a fun exercise that highlights the fundamental "selections" of D3--enter(), exit(), and merge().

I've modified Murray's code ([check it out on GitHub](https://github.com/scotthmurray/d3-book/blob/master/chapter_09/28_adding_and_removing.html)), adding buttons rather than paragraph elements, changing the style of the bars, and adding a dynamic x-axis to go along with the data. Check out the dynamic result at the bottom of this post.

{% include bar_chart_test.html %}

Code blocks, highlighted with [Prism](http://prismjs.com/index.html).

<pre><code class="language-markup">&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
&lt;head&gt;
	&lt;meta charset="utf-8" /&gt;
	&lt;title&gt;Dynamic Bar Chart with D3.js&lt;/title&gt;
	&lt;script src="https://d3js.org/d3.v5.js" &gt; &lt;/script&gt;
&lt;/head&gt;

&lt;body&gt;
  &lt;button class="button_click" id="add"&gt;Add a Bar&lt;/button&gt;
  &lt;button class="button_click" id="remove"&gt;Remove a Bar&lt;/button&gt;
  &lt;div id="chart"&gt;&lt;/div&gt;

  &lt;script type="text/javascript"&gt;

  var margin = ({top: 20, right: 30, bottom: 30, left: 40})

  var h = 300 - margin.top - margin.bottom;
  var w = 730 - margin.left - margin.right;

    var dataset = [
            { key: 0, value: 5 },
            { key: 1, value: 10 },
            { key: 2, value: 13 },
            { key: 3, value: 19 },
            { key: 4, value: 21 },
            { key: 5, value: 25 },
            { key: 6, value: 22 },
            { key: 7, value: 18 },
            { key: 8, value: 15 },
            { key: 9, value: 13 },
            { key: 10, value: 11 },
            { key: 11, value: 12 },
            { key: 12, value: 15 },
            { key: 13, value: 20 },
            { key: 14, value: 18 },
            { key: 15, value: 17 },
            { key: 16, value: 16 },
            { key: 17, value: 18 },
            { key: 18, value: 23 },
            { key: 19, value: 25 } ];

    var xScale = d3.scaleBand()
            .domain(d3.range(dataset.length))
            .rangeRound([0, w])
            .paddingInner(0.05);

    var yScale = d3.scaleLinear()
            .domain([0, d3.max(dataset, function(d) { return d.value; })])
            .range([0, h]);

    //Define key function, to be used when binding data
    var key = function(d) {
      return d.key;
    };

    //Create SVG element
    var svg = d3.select('#chart').append('svg')
      .attr("preserveAspectRatio", "xMinYMin meet")
      //.attr("viewBox", "-20 -20 " + w + " " + h)
      //this is to zoom out
      .attr("viewBox", "-20 -20 800 1000")
      .style("padding", 1)
      .style("margin", 1);

    var xAxis = svg.append("g")
            .attr('class', 'axis')
            .attr("transform", "translate(0," + (h) + ")")
            .call(d3.axisBottom(xScale).tickSizeOuter(0));

    //Create bars
    svg.selectAll("rect")
       .data(dataset, key)
       .enter()
       .append("rect")
       .attr("x", function(d, i) {
          return xScale(i);
       })
       .attr("y", function(d) {
          return h - yScale(d.value);
       })
       .attr("width", xScale.bandwidth())
       .attr("height", function(d) {
          return yScale(d.value);
       })
       .attr("fill", "steelblue");

    //Create labels
    svg.selectAll("text")
       .data(dataset, key)
       .enter()
       .append("text")
       .text(function(d) {
          return d.value;
       })
       .attr("text-anchor", "middle")
       .attr("x", function(d, i) {
          return xScale(i) + xScale.bandwidth() / 2;
       })
       .attr("y", function(d) {
          return h - yScale(d.value) + 14;
       })
       .attr("font-family", "sans-serif")
       .attr("font-size", "11px")
       .attr("fill", "white");


    //On click, update with new data
    d3.selectAll(".button_click")
      .on("click", function() {

        //See which p was clicked
        var buttonID = d3.select(this).attr("id");

        //Decide what to do next
        if (buttonID == "add") {
          //Add a data value
          var minValue = 2;
          var maxValue = 25 - minValue;
          var newNumber = Math.floor(Math.random() * maxValue) + minValue;
          var lastKeyValue = dataset[dataset.length - 1].key;
          dataset.push({
            key: lastKeyValue + 1,
            value: newNumber
          });
        } else {
          //Remove a value
          dataset.shift();	//Remove one value from dataset
        }

        //Update scale domains
        xScale.domain(d3.range(dataset.length));
        yScale.domain([0, d3.max(dataset, function(d) { return d.value; })]);

        //Select…
        var bars = svg.selectAll("rect")
          .data(dataset, key);

        var text = svg.selectAll("text")
          .data(dataset, key);

        var axis = svg.selectAll(".axis")
          .transition()
          .duration(500)
          .call(d3.axisBottom(xScale));

        //Enter…
        bars.enter()
          .append("rect")
          .attr("x", w)
          .attr("y", function(d) {
            return h - yScale(d.value);
          })
          .attr("width", xScale.bandwidth())
          .attr("height", function(d) {
            return yScale(d.value);
          })
          .attr("fill", "steelblue")
          .merge(bars)	//Update…
          .transition()
          .duration(500)
          .attr("x", function(d, i) {
            return xScale(i);
          })
          .attr("y", function(d) {
            return h - yScale(d.value);
          })
          .attr("width", xScale.bandwidth())
          .attr("height", function(d) {
            return yScale(d.value);
          });

        //Exit…
        bars.exit()
          .transition()
          .duration(500)
          .attr("x", -xScale.bandwidth())
          .remove();

        text.enter()
           .append("text")
           .text(function(d) {
              return d.value;
           })
           .attr("text-anchor", "middle")
           .attr("x", w)
           .attr("y", function(d) {
             return h - yScale(d.value);
           })
           .merge(text)
           .transition()
           .duration(500)
           .attr("x", function(d, i) {
              return xScale(i) + xScale.bandwidth() / 2;
           })
           .attr("y", function(d) {
              return h - yScale(d.value) + 14;
           });

        text.exit()
            .transition()
            .duration(500)
            .attr("x", -xScale.bandwidth())
            .remove();



        //Update all labels
        //
        //Exercise: Modify this code to add and remove the correct labels each time!
        //
        svg.selectAll("text")
           .data(dataset, key)
           .transition()
           .duration(500)
           .text(function(d) {
              return d.value;
           })
           .attr("x", function(d, i) {
            return xScale(i) + xScale.bandwidth() / 2;
           })
           .attr("y", function(d) {
            return h - yScale(d.value) + 14;
           });

      });


  &lt;/script&gt;
&lt;/body&gt;
&lt;/html&gt;

</code></pre>

And the styling, of course.

<pre><code class="language-css">@import url(http://fonts.googleapis.com/css?family=Arvo);

/* Styles */

    text {
      font: sans-serif;
      font-size: 12px;
      fill: white;
    }

    .button_click {
      color: white;
      height: 4em;
      width: 45%;
      padding: 0.5em auto;
      margin: 1em auto;
      background-color: #1d1d1d;
      border: none;
      border-radius: 3px;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      transition: all 0.2s cubic-bezier(.4,0,.2,1);
    }

    .button_click:hover {
      letter-spacing: 0.3em;
      background-color: #d4a25a;
    }

    .axis {
      stroke-width: 2px;
    }
    
}</code></pre>

