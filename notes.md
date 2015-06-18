What is D3?
===========

How can I learn D3?
===================

A Quick Overview
================

An SVG Primer
=============

An SVG Example
==============

CodePen source: http://codepen.io/uehreka/pen/waqZRK


D3 Selectors
============

Method Chaining
===============

Got it?
=======

**TODO**: This may need a little work. The example is a bit complicated and relies on a solid understanding of closures.
**TODO**: May want to write a few vertical slides in case we need more review

Keeping Track of Chained Methods
================================

**TODO**: May want to write a few vertical slides in case we need more review

Data Joins
==========

Data Selectors
==============

Not confusing at all
====================

The Enter Selector
==================

Demo of the Enter Selector

 - `svg.selectAll("circle")` - Select nothingness
 - `.data(data)` - Press Enter 3 times to make three spaces "There are 3 data points and 0 elements, so we set aside a space for each data point"
 - `.enter()` - "OK, now we're talking about the new data points that don't have elements yet"
 - `.attr("cx", function(d) { return d.xPos; })` 
    - Explain how the function gets mapped over the data points, this is a common D3 convention
    - Type `cx=""` and fill in the corresponding values
 - `.attr("cy", function(d) { return d.yPos; })` - Type `cy=""` and fill in the corresponding values
 - `.attr("r", 25)` - Type `r="25"` for each circle "If the second argument is a constant, we just use that."
 
Repeat again for adding a new data point

```
,
  {
    xPos:100,
    yPos:150
  }
```

Repeat again for changing an existing data point, to show that updates won't happen.

Repeat again for removing a data point, to show that exits won't happen.

Repeat again with appending `<rect>` elements, to show that the function won't be idempotent.

Enter, Update and Exit
======================

Add the new data point, and change 1 existing data point'

```
,
  {
    xPos:100,
    yPos:150
  }
```

**TODO**: Add a vertical slide showing how __data__ works under the hood

Scales
======


Color Scales
============

CodePen Example: http://codepen.io/uehreka/pen/ZGXOQP?editors=001

- Show the black to white color scale
- Replace the hex values with the rgb strings for red and blue
- Replace those with "red" and "blue"
- Replace those with the rainbow


Other Scale Topics
==================


Layouts
=======

**TODO**: Write about Layouts as media agnostic calculations

- Canvas + SVG Force Layout http://bl.ocks.org/sxv/4485778
- SVG Globe http://bl.ocks.org/mbostock/3795040
- Canvas Globe (Floating Landmasses) http://bl.ocks.org/mbostock/6738360
- Canvas Globe (Zooming and Panning) http://www.jasondavies.com/maps/zoom/

Let's Make a Bar Chart
======================

**TODO**: Walk through Bostock's tutorial