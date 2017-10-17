.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

quad()
======

วาดรูปสี่เหลี่ยมผืนผ้า รูปสี่เหลี่ยมเป็นรูปสี่เหลี่ยมผืนผ้าสี่เหลี่ยมรูปหลายเหลี่ยม มีลักษณะคล้ายกับรูปสี่เหลี่ยมผืนผ้า แต่มุมระหว่างขอบไม่ได้ จำกัด ไว้ที่ 90 องศา คู่แรกของพารามิเตอร์ (x1, y1) ตั้งค่าจุดสุดยอดแรกและคู่ที่ตามมาควรดำเนินการตามเข็มนาฬิกาหรือทวนเข็มนาฬิกาตามรูปร่างที่กำหนดไว้

.. Draw a quad. A quad is a quadrilateral, a four sided polygon. It is
.. similar to a rectangle, but the angles between its edges are not
.. constrained to ninety degrees. The first pair of parameters (x1,y1)
.. sets the first vertex and the subsequent pairs should proceed
.. clockwise or counter-clockwise around the defined shape.

**รูปแบบการใช้งาน**

quad ( x1, y1, x2, y2, x3, y3, x4, y4 )

**พารามิเตอร์**

- ``x1``  Number: พิกัด x ของจุดแรก

- ``y1``  Number: พิกัด y ของจุดแรก

- ``x2``  Number: พิกัด x ของจุดที่สอง

- ``y2``  Number: พิกัด y ของจุดที่สอง

- ``x3``  Number: พิกัด x ของจุดที่สาม

- ``y3``  Number: พิกัด y ของจุดที่สาม

- ``x4``  Number: พิกัด x ของจุดที่สี่

- ``y4``  Number: พิกัด y ของจุดที่สี่

.. ``x1``  Number: the x-coordinate of the first point
.. ``y1``  Number: the y-coordinate of the first point
.. ``x2``  Number: the x-coordinate of the second point
.. ``y2``  Number: the y-coordinate of the second point
.. ``x3``  Number: the x-coordinate of the third point
.. ``y3``  Number: the y-coordinate of the third point
.. ``x4``  Number: the x-coordinate of the fourth point
.. ``y4``  Number: the y-coordinate of the fourth point

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	quad(38, 31, 86, 20, 69, 63, 30, 76);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
