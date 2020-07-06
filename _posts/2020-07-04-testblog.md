---
layout: post
title: 'Blog Template'
tags: [JavaScript, Tips, D3.js]
featured_image_thumbnail:
featured_image:
featured: true
hidden: true
mathjax: true
---

Let's test some inline math $x$, $y$, $x_1$, $y_1$.

Now a inline math with special character: $|\psi\rangle$, $x'$, $x^\*$.

Test a display math:
$$
   |\psi_1\rangle = a|0\rangle + b|1\rangle
$$
Is it O.K.?

Test a display math with equation number:
\begin{equation}
   |\psi_1\rangle = a|0\rangle + b|1\rangle
\end{equation}

> "Insert quote here." <cite>- Speaker -</cite>

> this is a blockquote

Include figures:

HTML Code

<pre><code class="language-markup">
&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
&lt;head&gt;
    &lt;meta charset="utf-8" /&gt;
    &lt;title&gt;Prism&lt;/title&gt;
    &lt;link rel="stylesheet" href="style.css" /&gt;
&lt;/head&gt;
&lt;body&gt;
    &lt;header&gt;
        &lt;div class="intro" data-src="templates/header-main.html" data-type="text/html"&gt;&lt;/div&gt;
        &lt;ul id="features"&gt;
        &lt;li&gt;Dead simple&lt;/li&gt;
        &lt;li&gt;Light as a feather&lt;/li&gt;
        &lt;li&gt;Extensible&lt;/li&gt;
        &lt;/ul&gt;
    &lt;/header&gt;
    &lt;section id="features-full" class="language-markup"&gt;
        &lt;h1&gt;Full list of features&lt;/h1&gt;
        &lt;ul&gt;
            &lt;li&gt;&lt;strong&gt;Only 2KB&lt;/strong&gt; minified &amp; gzipped (core). Each language definition adds roughly 300-500 bytes.&lt;/li&gt;
            &lt;li&gt;Very easy to extend without modifying the code, due to Prism’s &lt;a href="#plugins"&gt;plugin architecture&lt;/a&gt;. Multiple hooks are scattered throughout the source.&lt;/li&gt;
            &lt;li&gt;Very easy to &lt;a href="extending.html#language-definitions"&gt;define new languages&lt;/a&gt;. Only thing you need is a good understanding of regular expressions&lt;/li&gt;
        &lt;/ul&gt;
    &lt;/section&gt;
    &lt;footer data-src="templates/footer.html" data-type="text/html"&gt;&lt;/footer&gt;
&lt;/body&gt;
&lt;/html&gt;
</code></pre>


JavaScript Code

<pre><code class="language-javascript">var Token = _.Token = function(type, content, alias, matchedStr, greedy) {
    this.type = type;
    this.content = content;
    this.alias = alias;
    // Copy of the full string this token was created from
    this.length = (matchedStr || "").length|0;
    this.greedy = !!greedy;
};</code></pre>


CSS Code

<pre><code class="language-css">

/* Styles */

body {
    font: 100%/1.5 Questrial, sans-serif;
    tab-size: 4;
    hyphens: auto;
}

a {
    color: inherit;
}

section h1 {
    font-size: 250%;
}

section h1,
#features li strong,
header h2,
footer p {
    font: 100% Rockwell, Arvo, serif;
}
</code></pre>

## Footnotes

The quick brown fox[^1] jumped over the lazy dog[^2].

[^1]: Foxes are red
[^2]: Dogs are usually not red

Footnotes are a great way to add additional contextual details when appropriate. Ghost will automatically add footnote content to the very end of your post.

## Tables

<table>
<caption>Table Caption</caption>
<thead>
<tr>
   <th>Content categories</th>
   <th>Flow content</th>
  </tr>
</thead>
 <tbody>
  <tr>
   <td>Permitted content</td>
   <td>
    An optional <code>&lt;caption&gt;</code> element;<br />
    zero or more <code>&lt;colgroup&gt;</code> elements;<br />
    an optional <code>&lt;thead&gt;</code> element;<br />
    an optional <code>&lt;tfoot&gt;</code> element;
   </td>
  </tr>
  <tr>
   <td>Tag omission</td>
   <td>None, both the start tag and the end tag are mandatory</td>
  </tr>
  <tr>
   <td>Permitted parent elements</td>
   <td>Any element that accepts flow content</td>
  </tr>
  <tr>
   <td>Normative document</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/tabular-data.html#the-table-element" rel="external nofollow">HTML5, section 4.9.1</a> (<a href="http://www.w3.org/TR/REC-html40/struct/tables.html#edef-TABLE">HTML4.01, section 11.2.1</a>)</td>
  </tr>
 </tbody>
</table>


## My effort to embed a custom D3.js viz


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
    .attr("r", 8)
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