Sketch Tape
===========

Sketch Tape is a plugin for Sketch that allows for connections to be made
between any two objects.

It accomplishes this by:

* Finding the midpoint of some object `a` and another object `b`.
* Find the midpoint between the two objects.
* Finding the angle between the midpoint in the middle to each of the other
  midpoints.
* Ray tracing from along this angle until an outside point on the shape is hit.
* Drawing a line between the two nearest outside points.

Usage
-----

Select two shapes in Sketch and hit ⌃-⌥-⇪-c.

Installation
------------

TODO

Limitations
-----------

* The two shapes must be within approximately 20,000 pixels of each other.
* It may fail to find an outside point on shapes with a lot of regions smaller
  than 1px in width.
* It will attempt to use the border style of the shape that is closer to the top
  of the list of layers. If that shape has no borders, it will try the second
  shape. If that fails, it will not attempt to draw the arrow.

TODO
----

* Finish installation section.
* Move the layer with the line to be behind the other two layers.
* Figure out a more sane approach to border styling.
* Add shortcuts for arrowheads etc.
