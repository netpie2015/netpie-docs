.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

curvePoint()
============

ประเมินเส้นโค้งที่ตำแหน่ง t สำหรับจุด a, b, c, d พารามิเตอร์ t แปรผันระหว่าง 0 และ 1, a และ d เป็นจุดบนเส้นโค้งและ b และ c เป็นจุดควบคุม นี้สามารถทำได้ครั้งเดียวกับพิกัด x และครั้งที่สองกับพิกัด y เพื่อให้ได้ตำแหน่งของเส้นโค้งที่ t

.. Evaluates the curve at position t for points a, b, c, d.
.. The parameter t varies between 0 and 1, a and d are points
.. on the curve, and b and c are the control points.
.. This can be done once with the x coordinates and a second time
.. with the y coordinates to get the location of a curve at t.

**รูปแบบการใช้งาน**

curvePoint ( a, b, c, d, t )

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

- Number: ค่า Bezier ที่ตำแหน่ง t

.. Number: bezier value at position t

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

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
