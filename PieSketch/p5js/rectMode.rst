.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

rectMode()
=============

ปรับเปลี่ยนตำแหน่งจากรูปสี่เหลี่ยมผืนผ้าที่วาดโดยการเปลี่ยนวิธีที่จะตีความพารามิเตอร์ที่กำหนดให้ rect ()

โหมดเริ่มต้นคือ rectMode (CORNER) ซึ่งจะตีความพารามิเตอร์สองค่าแรกของ rect () เป็นมุมซ้ายบนของรูปร่างในขณะที่พารามิเตอร์ที่สามและสี่คือความกว้างและความสูง

rectMode (CORNERS) ตีความพารามิเตอร์สองค่าแรกของ rect () เป็นตำแหน่งของมุมหนึ่งและพารามิเตอร์ที่สามและสี่เป็นตำแหน่งของมุมตรงข้าม

rectMode (CENTER) ตีความพารามิเตอร์สองค่าแรกของ rect () เป็นจุดกึ่งกลางของรูปร่างในขณะที่พารามิเตอร์ที่สามและสี่คือความกว้างและความสูง

rectMode (RADIUS) ใช้พารามิเตอร์สองตัวแรกของ rect () เป็นจุดกึ่งกลางของรูปร่าง แต่ใช้พารามิเตอร์ที่สามและสี่เพื่อระบุความกว้างและความสูงครึ่งหนึ่งของรูปร่าง

พารามิเตอร์ต้องเขียนเป็น CAPs เนื่องจาก Javascript เป็นภาษาที่ใช้ตัวพิมพ์เล็กและใหญ่

.. Modifies the location from which rectangles are drawn by changing the way in which parameters given to rect() are interpreted. 
.. The default mode is rectMode(CORNER), which interprets the first two parameters of rect() as the upper-left corner of the shape, while the third and fourth parameters are its width and height.
.. rectMode(CORNERS) interprets the first two parameters of rect() as the location of one corner, and the third and fourth parameters as the location of the opposite corner.
.. rectMode(CENTER) interprets the first two parameters of rect() as the shape's center point, while the third and fourth parameters are its width and height. 
.. rectMode(RADIUS) also uses the first two parameters of rect() as the shape's center point, but uses the third and fourth parameters to specify half of the shapes's width and height. 
.. The parameter must be written in ALL CAPS because Javascript is a case-sensitive language.

**รูปแบบการใช้งาน**

rectMode(mode)

**พารามิเตอร์**

- ``mode``  ค่าคงที่: CORNER, CORNERS, CENTER หรือ RADIUS

.. - ``mode``  either CORNER, CORNERS, CENTER, or RADIUS

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	rectMode(CORNER);  // Default rectMode is CORNER
    fill(255);  // Set fill to white
    rect(25, 25, 50, 50);  // Draw white rect using CORNER mode

    rectMode(CORNERS);  // Set rectMode to CORNERS
    fill(100);  // Set fill to gray
    rect(25, 25, 50, 50);  // Draw gray rect using CORNERS mode
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	rectMode(RADIUS);  // Set rectMode to RADIUS
    fill(255);  // Set fill to white
    rect(50, 50, 30, 30);  // Draw white rect using RADIUS mode

    rectMode(CENTER);  // Set rectMode to CENTER
    fill(100);  // Set fill to gray
    rect(50, 50, 30, 30);  // Draw gray rect using CENTER mode
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
