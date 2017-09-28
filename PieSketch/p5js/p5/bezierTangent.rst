.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

bezierTangent()
===============

ประเมินจุดสัมผัสกับ Bezier ที่ตำแหน่ง t สำหรับจุด a, b, c, d พารามิเตอร์ a และ d เป็นจุดแรกและจุดสุดท้ายของเส้นโค้งและ b และ c เป็นจุดควบคุม พารามิเตอร์สุดท้าย t แปรผันระหว่าง 0 และ 1

.. Evaluates the tangent to the Bezier at position t for points a, b, c, d.
.. The parameters a and d are the first and last points
.. on the curve, and b and c are the control points.
.. The final parameter t varies between 0 and 1.

**รูปแบบการใช้งาน**

bezierTangent ( a, b, c, d, t )

**พารามิเตอร์**

- ``a``  Number: พิกัดของจุดแรกบนเส้นโค้ง

- ``b``  Number: พิกัดของจุดควบคุมแรก

- ``c``  Number: พิกัดของจุดควบคุมที่สอง

- ``d``  Number: พิกัดของจุดที่สองบนเส้นโค้ง

- ``t``  Number: ค่าระหว่าง 0 ถึง 1

.. ``a``  Number: coordinate of first point on the curve
.. ``b``  Number: coordinate of first control point
.. ``c``  Number: coordinate of second control point
.. ``d``  Number: coordinate of second point on the curve
.. ``t``  Number: value between 0 and 1

**ค่าที่ส่งออกมา**

- Number: สัมผัสกันที่ตำแหน่ง t

.. Number: the tangent at position t

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	bezier(85, 20, 10, 10, 90, 90, 15, 80);
	steps = 6;
	fill(255);
	for (i = 0; i <= steps; i++) {
	  t = i / steps;
	  // Get the location of the point
	  x = bezierPoint(85, 10, 90, 15, t);
	  y = bezierPoint(20, 10, 90, 80, t);
	  // Get the tangent points
	  tx = bezierTangent(85, 10, 90, 15, t);
	  ty = bezierTangent(20, 10, 90, 80, t);
	  // Calculate an angle from the tangent points
	  a = atan2(ty, tx);
	  a += PI;
	  stroke(255, 102, 0);
	  line(x, y, cos(a)*30 + x, sin(a)*30 + y);
	  // The following line of code makes a line
	  // inverse of the above line
	  //line(x, y, cos(a)*-30 + x, sin(a)*-30 + y);
	  stroke(0);
	  ellipse(x, y, 5, 5);
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	noFill();
	bezier(85, 20, 10, 10, 90, 90, 15, 80);
	stroke(255, 102, 0);
	steps = 16;
	for (i = 0; i <= steps; i++) {
	  t = i / steps;
	  x = bezierPoint(85, 10, 90, 15, t);
	  y = bezierPoint(20, 10, 90, 80, t);
	  tx = bezierTangent(85, 10, 90, 15, t);
	  ty = bezierTangent(20, 10, 90, 80, t);
	  a = atan2(ty, tx);
	  a -= HALF_PI;
	  line(x, y, cos(a)*8 + x, sin(a)*8 + y);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
