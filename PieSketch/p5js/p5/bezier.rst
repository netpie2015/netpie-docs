.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

bezier()
========

วาดโค้ง Bezier ลูกบาศก์บนหน้าจอ เส้นโค้งเหล่านี้ถูกกำหนดโดยชุดจุดยึดและจุดควบคุม พารามิเตอร์สองตัวแรกระบุจุดยึดแรกและพารามิเตอร์สองตัวสุดท้ายระบุจุดยึดอื่น ๆ ซึ่งจะกลายเป็นจุดแรกและจุดสุดท้ายของเส้นโค้ง พารามิเตอร์กลางระบุจุดควบคุมสองจุดที่กำหนดรูปร่างของเส้นโค้ง ประมาณพูดจุดควบคุม "ดึง" เส้นโค้งไปทางพวกเขา  เส้นโค้ง Bezier ได้รับการพัฒนาโดยวิศวกรชาวฝรั่งเศส Pierre Bezier และมักใช้กราฟิกคอมพิวเตอร์เพื่อกำหนดเส้นโค้งที่ลาดเอียงเล็กน้อย ดูเพิ่มเติมที่ curve ()

.. Draws a cubic Bezier curve on the screen. These curves are defined by a
.. series of anchor and control points. The first two parameters specify
.. the first anchor point and the last two parameters specify the other
.. anchor point, which become the first and last points on the curve. The
.. middle parameters specify the two control points which define the shape
.. of the curve. Approximately speaking, control points "pull" the curve
.. towards them.Bezier curves were developed by French
.. automotive engineer Pierre Bezier, and are commonly used in computer
.. graphics to define gently sloping curves. See also curve().

**รูปแบบการใช้งาน**

bezier ( x1, y1, x2, y2, x3, y3, x4, y4 )

**พารามิเตอร์**

- ``x1``  Number: พิกัด x สำหรับจุดยึดแรก

- ``y1``  Number: พิกัด y สำหรับจุดยึดแรก

- ``x2``  Number: พิกัด x สำหรับจุดควบคุมแรก

- ``y2``  Number: y พิกัดสำหรับจุดควบคุมแรก

- ``x3``  Number: พิกัด x สำหรับจุดควบคุมที่สอง

- ``y3``  Number: y พิกัดสำหรับจุดควบคุมที่สอง

- ``x4``  Number: พิกัด x สำหรับจุดยึดที่สอง

- ``y4``  Number: y- พิกัดสำหรับจุดยึดที่สอง

.. ``x1``  Number: x-coordinate for the first anchor point
.. ``y1``  Number: y-coordinate for the first anchor point
.. ``x2``  Number: x-coordinate for the first control point
.. ``y2``  Number: y-coordinate for the first control point
.. ``x3``  Number: x-coordinate for the second control point
.. ``y3``  Number: y-coordinate for the second control point
.. ``x4``  Number: x-coordinate for the second anchor point
.. ``y4``  Number: y-coordinate for the second anchor point

**ค่าที่ส่งออกมา**

- p5: วัตถุ p5

.. p5: the p5 object

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	stroke(255, 102, 0);
	line(85, 20, 10, 10);
	line(90, 90, 15, 80);
	stroke(0, 0, 0);
	bezier(85, 20, 10, 10, 90, 90, 15, 80);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
