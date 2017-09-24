.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

curveTangent()
==============

Evaluates the tangent to the curve at position t for points a, b, c, d.
The parameter t varies between 0 and 1, a and d are points on the curve,
and b and c are the control points.

**รูปแบบการใช้งาน**

curveTangent ( a, b, c, d, t )

**พารามิเตอร์**

- ``a``  Number: coordinate of first point on the curve

- ``b``  Number: coordinate of first control point

- ``c``  Number: coordinate of second control point

- ``d``  Number: coordinate of second point on the curve

- ``t``  Number: value between 0 and 1


**ค่าที่ส่งออกมา**

- Number: the tangent at position t


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	curve(5, 26, 73, 24, 73, 61, 15, 65);
	steps = 6;
	for (i = 0; i <= steps; i++) {
	  t = i / steps;
	  x = curvePoint(5, 73, 73, 15, t);
	  y = curvePoint(26, 24, 61, 65, t);
	  //ellipse(x, y, 5, 5);
	  tx = curveTangent(5, 73, 73, 15, t);
	  ty = curveTangent(26, 24, 61, 65, t);
	  a = atan2(ty, tx);
	  a -= PI/2.0;
	  line(x, y, cos(a)*8 + x, sin(a)*8 + y);
	}


	</script>

	<br><br>

.. toctree::

