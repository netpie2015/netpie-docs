.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

bezierVertex()
==============

Specifies vertex coordinates for Bezier curves. Each call to
bezierVertex() defines the position of two control points and
one anchor point of a Bezier curve, adding a new segment to a
line or shape.

The first time bezierVertex() is used within a
beginShape() call, it must be prefaced with a call to vertex()
to set the first anchor point. This function must be used between
beginShape() and endShape() and only when there is no MODE
parameter specified to beginShape().

**รูปแบบการใช้งาน**

bezierVertex ( x2, y2, x3, y3, x4, y4 )

**พารามิเตอร์**

- ``x2``  Number: x-coordinate for the first control point

- ``y2``  Number: y-coordinate for the first control point

- ``x3``  Number: x-coordinate for the second control point

- ``y3``  Number: y-coordinate for the second control point

- ``x4``  Number: x-coordinate for the anchor point

- ``y4``  Number: y-coordinate for the anchor point


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	beginShape();
	vertex(30, 20);
	bezierVertex(80, 0, 80, 75, 30, 75);
	endShape();


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	beginShape();
	vertex(30, 20);
	bezierVertex(80, 0, 80, 75, 30, 75);
	bezierVertex(50, 80, 60, 25, 30, 20);
	endShape();


	</script>

	<br><br>

.. toctree::

