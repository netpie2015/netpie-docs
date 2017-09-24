.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

curve()
=======

Draws a curved line on the screen between two points, given as the
middle four parameters. The first two parameters are a control point, as
if the curve came from this point even though it's not drawn. The last
two parameters similarly describe the other control point. 
Longer curves can be created by putting a series of curve() functions
together or using curveVertex(). An additional function called
curveTightness() provides control for the visual quality of the curve.
The curve() function is an implementation of Catmull-Rom splines.

**รูปแบบการใช้งาน**

curve ( x1, y1, x2, y2, x3, y3, x4, y4 )

**พารามิเตอร์**

- ``x1``  Number: x-coordinate for the beginning control point

- ``y1``  Number: y-coordinate for the beginning control point

- ``x2``  Number: x-coordinate for the first point

- ``y2``  Number: y-coordinate for the first point

- ``x3``  Number: x-coordinate for the second point

- ``y3``  Number: y-coordinate for the second point

- ``x4``  Number: x-coordinate for the ending control point

- ``y4``  Number: y-coordinate for the ending control point


**ค่าที่ส่งออกมา**

- p5: the p5 object


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	stroke(255, 102, 0);
	curve(5, 26, 5, 26, 73, 24, 73, 61);
	stroke(0);
	curve(5, 26, 73, 24, 73, 61, 15, 65);
	stroke(255, 102, 0);
	curve(73, 24, 73, 61, 15, 65, 15, 65);


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Define the curve points as JavaScript objects
	p1 = {x: 5, y: 26}, p2 = {x: 73, y: 24}
	p3 = {x: 73, y: 61}, p4 = {x: 15, y: 65}
	noFill();
	stroke(255, 102, 0);
	curve(p1.x, p1.y, p1.x, p1.y, p2.x, p2.y, p3.x, p3.y)
	stroke(0);
	curve(p1.x, p1.y, p2.x, p2.y, p3.x, p3.y, p4.x, p4.y)
	stroke(255, 102, 0);
	curve(p2.x, p2.y, p3.x, p3.y, p4.x, p4.y, p4.x, p4.y)


	</script>

	<br><br>

.. toctree::

