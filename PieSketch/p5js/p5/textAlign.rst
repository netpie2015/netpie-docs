.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

textAlign()
===========

ตั้งค่าการจัดตำแหน่งปัจจุบันสำหรับการวาดข้อความ ยอมรับอาร์กิวเมนต์สองตัว: horizAlign (ซ้ายขวากลางและขวา) และ vertAlign (TOP, BOTTOM, CENTER หรือ BASELINE) พารามิเตอร์ horizAlign อ้างอิงถึงค่า x ของข้อความ () ฟังก์ชันในขณะที่พารามิเตอร์ vertAlign อยู่ในการอ้างอิงถึงค่า y ดังนั้นหากคุณเขียน textAlign (LEFT) คุณจะจัดเรียงขอบด้านซ้ายของข้อความให้เป็นค่า x ที่คุณให้ไว้ในข้อความ () หากคุณเขียน textAlign (RIGHT, TOP) คุณจะจัดเรียงขอบด้านขวาของข้อความให้เป็นค่า x และด้านบนของขอบของข้อความเป็นค่า y

.. Sets the current alignment for drawing text. Accepts two
.. arguments: horizAlign (LEFT, CENTER, or RIGHT) and
.. vertAlign (TOP, BOTTOM, CENTER, or BASELINE).
.. The horizAlign parameter is in reference to the x value
.. of the text() function, while the vertAlign parameter is
.. in reference to the y value.
.. So if you write textAlign(LEFT), you are aligning the left
.. edge of your text to the x value you give in text(). If you
.. write textAlign(RIGHT, TOP), you are aligning the right edge
.. of your text to the x value and the top of edge of the text
.. to the y value.

**รูปแบบการใช้งาน**

textAlign ( horizAlign, [vertAlign] )

**พารามิเตอร์**

- ``horizAlign``  Constant: แนวนอนทั้งซ้าย, กลางหรือขวา

- ``vertAlign``  Constant: การจัดแนวแนวตั้งทั้ง TOP, BOTTOM, CENTER หรือ BASELINE

.. ``horizAlign``  Constant: horizontal alignment, either LEFT, CENTER, or RIGHT
.. ``vertAlign``  Constant: vertical alignment, either TOP, BOTTOM, CENTER, or BASELINE

**ค่าที่ส่งออกมา**

- Number: 

.. Number: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	textSize(16);
	textAlign(RIGHT);
	text("ABCD", 50, 30);
	textAlign(CENTER);
	text("EFGH", 50, 50);
	textAlign(LEFT);
	text("IJKL", 50, 70);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
