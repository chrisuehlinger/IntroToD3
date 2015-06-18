What is D3?
===========


How can I learn D3?
===================

A Quick Overview
================

An SVG Primer
=============

D3 Selectors
============

Method Chaining
===============

Got it?
=======

**TODO**: This may need a little work

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

**TODO**: Write about Scales as transparent functions


Layouts
=======

**TODO**: Write about Layouts as media agnostic calculations

