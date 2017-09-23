.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

curvePoint()
============

Evaluates the curve at position t for points a, b, c, d.
The parameter t varies between 0 and 1, a and d are points
on the curve, and b and c are the control points.
This can be done once with the x coordinates and a second time
with the y coordinates to get the location of a curve at t.

**รูปแบบการใช้งาน**

curvePoint ( a, b, c, d, t )

**พารามิเตอร์**

- ``a``  : coordinate of first point on the curve

- ``b``  : coordinate of first control point

- ``c``  : coordinate of second control point

- ``d``  : coordinate of second point on the curve

- ``t``  : value between 0 and 1


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	curve(5, 26, 5, 26, 73, 24, 73, 61);
	curve(5, 26, 73, 24, 73, 61, 15, 65);
	fill(255);
	ellipseMode(CENTER);
	steps = 6;
	for (i = 0; i <= steps; i++) {
	  t = i / steps;
	  x = curvePoint(5, 5, 73, 73, t);
	  y = curvePoint(26, 26, 24, 61, t);
	  ellipse(x, y, 5, 5);
	  x = curvePoint(5, 73, 73, 15, t);
	  y = curvePoint(26, 24, 61, 65, t);
	  ellipse(x, y, 5, 5);
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	line hooking down to right-bottom with 13 5x5 white ellipse points
	</script>

	<br><br>

.. toctree::

