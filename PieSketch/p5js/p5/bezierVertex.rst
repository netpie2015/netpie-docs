.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

bezierVertex()
==============

ระบุพิกัดจุดสุดยอดสำหรับเส้นโค้ง Bezier การเรียกไปยัง bezierVertex () จะกำหนดตำแหน่งของจุดควบคุมสองจุดและจุดยึดหนึ่งเส้นของเส้นโค้ง Bezier เพิ่มส่วนใหม่ลงในเส้นหรือรูปร่าง 
ครั้งแรก bezierVertex () จะถูกใช้ภายในการโทรแบบ beginShape () จะต้องมีการโทรไปยังจุดยอด () เพื่อตั้งจุดยึดแรก ต้องใช้ฟังก์ชันนี้ระหว่าง BeginShape () และ endShape () และเฉพาะเมื่อไม่มีพารามิเตอร์ MODE ที่ระบุเพื่อเริ่มต้น Shape ()

.. Specifies vertex coordinates for Bezier curves. Each call to
.. bezierVertex() defines the position of two control points and
.. one anchor point of a Bezier curve, adding a new segment to a
.. line or shape.
.. 
.. The first time bezierVertex() is used within a
.. beginShape() call, it must be prefaced with a call to vertex()
.. to set the first anchor point. This function must be used between
.. beginShape() and endShape() and only when there is no MODE
.. parameter specified to beginShape().
**รูปแบบการใช้งาน**

bezierVertex ( x2, y2, x3, y3, x4, y4 )

**พารามิเตอร์**

- ``x2``  Number: พิกัด x สำหรับจุดควบคุมแรก

- ``y2``  Number: y พิกัดสำหรับจุดควบคุมแรก

- ``x3``  Number: พิกัด x สำหรับจุดควบคุมที่สอง

- ``y3``  Number: y พิกัดสำหรับจุดควบคุมที่สอง

- ``x4``  Number: พิกัด x สำหรับจุดยึด

- ``y4``  Number: พิกัด y สำหรับจุดยึด

.. ``x2``  Number: x-coordinate for the first control point
.. ``y2``  Number: y-coordinate for the first control point
.. ``x3``  Number: x-coordinate for the second control point
.. ``y3``  Number: y-coordinate for the second control point
.. ``x4``  Number: x-coordinate for the anchor point
.. ``y4``  Number: y-coordinate for the anchor point

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

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
