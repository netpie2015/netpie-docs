.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

quadraticVertex()
=================

Specifies vertex coordinates for quadratic Bezier curves. Each call to
quadraticVertex() defines the position of one control points and one
anchor point of a Bezier curve, adding a new segment to a line or shape.
The first time quadraticVertex() is used within a beginShape() call, it
must be prefaced with a call to vertex() to set the first anchor point.
This function must be used between beginShape() and endShape() and only
when there is no MODE parameter specified to beginShape().

**รูปแบบการใช้งาน**

quadraticVertex ( cx, cy, x3, y3 )

**พารามิเตอร์**

- ``cx``  Number: x-coordinate for the control point

- ``cy``  Number: y-coordinate for the control point

- ``x3``  Number: x-coordinate for the anchor point

- ``y3``  Number: y-coordinate for the anchor point


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	strokeWeight(4);
	beginShape();
	vertex(20, 20);
	quadraticVertex(80, 20, 50, 50);
	endShape();

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	noFill();
	strokeWeight(4);
	beginShape();
	vertex(20, 20);
	quadraticVertex(80, 20, 50, 50);
	quadraticVertex(20, 80, 80, 80);
	vertex(80, 60);
	endShape();

	</script>

	<br><br>

.. toctree::

