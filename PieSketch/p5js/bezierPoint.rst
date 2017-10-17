.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

bezierPoint()
=============

ประเมิน Bezier ที่ตำแหน่ง t สำหรับจุด a, b, c, d พารามิเตอร์ a และ d เป็นจุดแรกและจุดสุดท้ายของเส้นโค้งและ b และ c เป็นจุดควบคุม พารามิเตอร์สุดท้าย t แตกต่างกันระหว่าง 0 ถึง 1 ซึ่งสามารถทำได้ครั้งเดียวกับพิกัด x และครั้งที่สองโดยใช้พิกัด y เพื่อหาตำแหน่งของเส้นโค้ง Bezier ที่ t

.. Evaluates the Bezier at position t for points a, b, c, d.
.. The parameters a and d are the first and last points
.. on the curve, and b and c are the control points.
.. The final parameter t varies between 0 and 1.
.. This can be done once with the x coordinates and a second time
.. with the y coordinates to get the location of a bezier curve at t.

**รูปแบบการใช้งาน**

bezierPoint ( a, b, c, d, t )

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

- Number: ค่าของ Bezier ที่ตำแหน่ง t

.. Number: the value of the Bezier at position t

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	x1 = 85, x2 = 10, x3 = 90, x4 = 15;
	y1 = 20, y2 = 10, y3 = 90, y4 = 80;
	bezier(x1, y1, x2, y2, x3, y3, x4, y4);
	fill(255);
	steps = 10;
	for (i = 0; i <= steps; i++) {
	  t = i / steps;
	  x = bezierPoint(x1, x2, x3, x4, t);
	  y = bezierPoint(y1, y2, y3, y4, t);
	  ellipse(x, y, 5, 5);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
