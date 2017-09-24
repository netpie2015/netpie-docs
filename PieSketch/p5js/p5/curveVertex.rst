.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

curveVertex()
=============

Specifies vertex coordinates for curves. This function may only
be used between beginShape() and endShape() and only when there
is no MODE parameter specified to beginShape().

The first and last points in a series of curveVertex() lines will be used to
guide the beginning and end of a the curve. A minimum of four
points is required to draw a tiny curve between the second and
third points. Adding a fifth point with curveVertex() will draw
the curve between the second, third, and fourth points. The
curveVertex() function is an implementation of Catmull-Rom
splines.

**รูปแบบการใช้งาน**

curveVertex ( x, y )

**พารามิเตอร์**

- ``x``  Number: x-coordinate of the vertex

- ``y``  Number: y-coordinate of the vertex


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	beginShape();
	curveVertex(84,  91);
	curveVertex(84,  91);
	curveVertex(68,  19);
	curveVertex(21,  17);
	curveVertex(32, 100);
	curveVertex(32, 100);
	endShape();


	</script>

	<br><br>

.. toctree::

