.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

quadraticVertex()
=================

ระบุพิกัดจุดสุดยอดสำหรับเส้นโค้ง Bezier แบบสี่เหลี่ยม การโทรไปยัง quadraticVertex () จะกำหนดตำแหน่งของจุดควบคุมหนึ่งจุดและจุดยึดหนึ่งเส้นของเส้นโค้ง Bezier เพิ่มส่วนใหม่ลงในเส้นหรือรูปร่าง ครั้งแรก quadraticVertex () จะถูกใช้ภายในการโทรเริ่มต้น () คุณต้องใส่คำนำหน้าไปยังจุดยอด () เพื่อตั้งจุดสมอแรก ต้องใช้ฟังก์ชันนี้ระหว่าง BeginShape () และ endShape () และเฉพาะเมื่อไม่มีพารามิเตอร์ MODE ที่ระบุเพื่อเริ่มต้น Shape ()

.. Specifies vertex coordinates for quadratic Bezier curves. Each call to
.. quadraticVertex() defines the position of one control points and one
.. anchor point of a Bezier curve, adding a new segment to a line or shape.
.. The first time quadraticVertex() is used within a beginShape() call, it
.. must be prefaced with a call to vertex() to set the first anchor point.
.. This function must be used between beginShape() and endShape() and only
.. when there is no MODE parameter specified to beginShape().

**รูปแบบการใช้งาน**

quadraticVertex ( cx, cy, x3, y3 )

**พารามิเตอร์**

- ``cx``  Number: พิกัด x สำหรับจุดควบคุม

- ``cy``  Number: พิกัด y สำหรับจุดควบคุม

- ``x3``  Number: พิกัด x สำหรับจุดยึด

- ``y3``  Number: พิกัด y สำหรับจุดยึด

.. ``cx``  Number: x-coordinate for the control point
.. ``cy``  Number: y-coordinate for the control point
.. ``x3``  Number: x-coordinate for the anchor point
.. ``y3``  Number: y-coordinate for the anchor point

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

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
