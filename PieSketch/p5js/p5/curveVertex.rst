.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

curveVertex()
=============

ระบุพิกัดจุดสุดยอดสำหรับเส้นโค้ง ฟังก์ชันนี้ใช้ได้เฉพาะระหว่าง beginShape () และ endShape () เท่านั้นเมื่อไม่มีพารามิเตอร์ MODE ที่ระบุเพื่อเริ่มต้นรูปร่าง () 
จุดแรกและจุดสุดท้ายในชุดเส้นโค้ง () จะถูกใช้เพื่อเป็นแนวทางในการเริ่มต้นและจุดสิ้นสุดของเส้นโค้ง ต้องใช้จุดอย่างน้อยสี่จุดเพื่อวาดเส้นโค้งเล็ก ๆ ระหว่างจุดที่สองและจุดที่สาม การเพิ่มจุดที่ห้าด้วย curveVertex () จะวาดเส้นโค้งระหว่างจุดที่สองสามและสี่ ฟังก์ชัน curveVertex () คือการดำเนินการ Splines Catmull-Rom

.. Specifies vertex coordinates for curves. This function may only
.. be used between beginShape() and endShape() and only when there
.. is no MODE parameter specified to beginShape().
.. 
.. The first and last points in a series of curveVertex() lines will be used to
.. guide the beginning and end of a the curve. A minimum of four
.. points is required to draw a tiny curve between the second and
.. third points. Adding a fifth point with curveVertex() will draw
.. the curve between the second, third, and fourth points. The
.. curveVertex() function is an implementation of Catmull-Rom
.. splines.

**รูปแบบการใช้งาน**

curveVertex ( x, y )

**พารามิเตอร์**

- ``x``  Number: พิกัด x ของจุดสุดยอด

- ``y``  Number: y พิกัดของจุดยอด

.. ``x``  Number: x-coordinate of the vertex
.. ``y``  Number: y-coordinate of the vertex

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	beginShape();
	curveVertex(84,  91);
	curveVertex(84,  91);
	curveVertex(68,  19);
	curveVertex(21,  17);
	curveVertex(32, 100);
	curveVertex(32, 100);
	endShape();

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
