.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

line()
======

วาดเส้น (เส้นทางตรงระหว่างจุดสองจุด) ไปยังหน้าจอ รุ่นของบรรทัด () ที่มีสี่พารามิเตอร์วาดเส้นในรูปแบบ 2D เมื่อต้องการทำสีเส้นให้ใช้ฟังก์ชัน stroke () ไม่สามารถเติมเส้นได้ดังนั้นฟังก์ชัน fill () จะไม่ส่งผลต่อสีของเส้น เส้น 2D จะวาดด้วยความกว้างหนึ่งพิกเซลตามค่าเริ่มต้น แต่สามารถเปลี่ยนแปลงได้ด้วยฟังก์ชัน strokeWeight ()

.. Draws a line (a direct path between two points) to the screen. The version
.. of line() with four parameters draws the line in 2D. To color a line, use
.. the stroke() function. A line cannot be filled, therefore the fill()
.. function will not affect the color of a line. 2D lines are drawn with a
.. width of one pixel by default, but this can be changed with the
.. strokeWeight() function.

**รูปแบบการใช้งาน**

line ( x1, y1, x2, y2 )

**พารามิเตอร์**

- ``x1``  Number: พิกัด x ของจุดแรก

- ``y1``  Number: พิกัด y ของจุดแรก

- ``x2``  Number: พิกัด x ของจุดที่สอง

- ``y2``  Number: พิกัด y ของจุดที่สอง

.. ``x1``  Number: the x-coordinate of the first point
.. ``y1``  Number: the y-coordinate of the first point
.. ``x2``  Number: the x-coordinate of the second point
.. ``y2``  Number: the y-coordinate of the second point

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	line(30, 20, 85, 75);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	line(30, 20, 85, 20);
	stroke(126);
	line(85, 20, 85, 75);
	stroke(255);
	line(85, 75, 30, 75);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
