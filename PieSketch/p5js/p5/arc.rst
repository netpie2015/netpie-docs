.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

arc()
=====

วาดส่วนโค้งไปที่หน้าจอ ถ้าเรียกว่ามีเฉพาะ a, b, c, d, เริ่มต้นและหยุด, ส่วนโค้งจะวาดเป็นพายเปิด หากมีการจัดเตรียมโหมดไว้ส่วนโค้งจะวาดทั้งแบบเปิดเป็นคอร์ดหรือเป็นพายตามที่ระบุ ต้นกำเนิดอาจเปลี่ยนแปลงได้โดยใช้ฟังก์ชัน ellipseMode () 
โปรดทราบว่าการวาดวงกลมแบบเต็ม (เช่น: 0 ถึง TWO_PI) จะปรากฏเป็นค่าว่างเนื่องจาก 0 และ TWO_PI เป็นตำแหน่งเดียวกันกับวงกลมหน่วย วิธีที่ดีที่สุดในการจัดการนี้คือการใช้ฟังก์ชัน ellipse () แทนที่จะสร้างวงรีที่ปิดและใช้ฟังก์ชัน arc () เพื่อวาดส่วนของวงรี

.. Draw an arc to the screen. If called with only a, b, c, d, start, and
.. stop, the arc will be drawn as an open pie. If mode is provided, the arc
.. will be drawn either open, as a chord, or as a pie as specified. The
.. origin may be changed with the ellipseMode() function.
.. 
.. Note that drawing a full circle (ex: 0 to TWO_PI) will appear blank
.. because 0 and TWO_PI are the same position on the unit circle. The
.. best way to handle this is by using the ellipse() function instead
.. to create a closed ellipse, and to use the arc() function
.. only to draw parts of an ellipse.

**รูปแบบการใช้งาน**

arc ( a, b, c, d, start, stop, [mode] )

**พารามิเตอร์**

- ``a``  Number: x- พิกัดของวงรีโค้ง

- ``b``  Number: y พิกัดของวงรีโค้ง

- ``c``  Number: ความกว้างของวงรีโค้งโดยค่าเริ่มต้น

- ``d``  Number: ความสูงของวงรีโค้งโดยค่าเริ่มต้น

- ``start``  Number: มุมเพื่อเริ่มโค้งซึ่งระบุเป็นเรเดียน

- ``stop``  Number: มุมเพื่อหยุดส่วนโค้งที่ระบุไว้เป็นเรเดียน

- ``mode``  Constant: พารามิเตอร์ตัวเลือกเพื่อกำหนดวิธีวาดเส้นโค้ง ทั้ง CHORD หรือ PIE

.. ``a``  Number: x-coordinate of the arc's ellipse
.. ``b``  Number: y-coordinate of the arc's ellipse
.. ``c``  Number: width of the arc's ellipse by default
.. ``d``  Number: height of the arc's ellipse by default
.. ``start``  Number: angle to start the arc, specified in radians
.. ``stop``  Number: angle to stop the arc, specified in radians
.. ``mode``  Constant: optional parameter to determine the way of drawing the arc. either CHORD or PIE

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	arc(50, 55, 50, 50, 0, HALF_PI);
	noFill();
	arc(50, 55, 60, 60, HALF_PI, PI);
	arc(50, 55, 70, 70, PI, PI+QUARTER_PI);
	arc(50, 55, 80, 80, PI+QUARTER_PI, TWO_PI);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	arc(50, 50, 80, 80, 0, PI+QUARTER_PI, OPEN);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	arc(50, 50, 80, 80, 0, PI+QUARTER_PI, CHORD);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	arc(50, 50, 80, 80, 0, PI+QUARTER_PI, PIE);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
