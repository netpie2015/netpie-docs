.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

ellipseMode()
=============

แก้ไขตำแหน่งที่ตั้งจากจุดศูนย์กลางที่ถูกวาดโดยการเปลี่ยนวิธีการตีความตัวแปรที่ให้กับวงรี ()

โหมดค่าเริ่มต้นคือ ellipseMode (CENTER) ซึ่งจะตีความตัวแปรสองค่าแรกของรูปวงรี () เป็นจุดกึ่งกลางของรูปร่างในขณะที่พารามิเตอร์ที่สามและสี่คือความกว้างและความสูง

ellipseMode (RADIUS) ใช้พารามิเตอร์สองตัวแรกของวงรี () เป็นจุดกึ่งกลางของรูปร่าง แต่ใช้พารามิเตอร์ที่สามและสี่เพื่อระบุความกว้างและความสูงครึ่งหนึ่งของรูปทรง

ellipseMode (CORNER) ตีความพารามิเตอร์สองตัวแรกของวงรี () เป็นมุมซ้ายบนของรูปร่างในขณะที่พารามิเตอร์ที่สามและสี่มีความกว้างและความสูง

ellipseMode (CORNERS) ตีความพารามิเตอร์สองตัวแรกของรูปวงรี () เป็นตำแหน่งของมุมหนึ่งของกรอบขอบเขตของรูปวงรีและพารามิเตอร์ที่สามและสี่เป็นตำแหน่งของมุมตรงข้าม

พารามิเตอร์ต้องเขียนเป็น CAPs เนื่องจาก Javascript เป็นภาษาที่ใช้ตัวพิมพ์เล็กและใหญ่

.. Modifies the location from which ellipses are drawn by changing the way in which parameters given to ellipse() are interpreted. 
.. The default mode is ellipseMode(CENTER), which interprets the first two parameters of ellipse() as the shape's center point, while the third and fourth parameters are its width and height. 
.. ellipseMode(RADIUS) also uses the first two parameters of ellipse() as the shape's center point, but uses the third and fourth parameters to specify half of the shapes's width and height.
.. ellipseMode(CORNER) interprets the first two parameters of ellipse() as the upper-left corner of the shape, while the third and fourth parameters are its width and height. 
.. 
.. ellipseMode(CORNERS) interprets the first two parameters of ellipse() as the location of one corner of the ellipse's bounding box, and the third and fourth parameters as the location of the opposite corner. 
.. The parameter must be written in ALL CAPS because Javascript is a case-sensitive language.

**รูปแบบการใช้งาน**

ellipseMode(mode)

**พารามิเตอร์**

- ``mode``  ค่าคงที่: ไม่ว่าจะเป็น CENTER, RADIUS, CORNER หรือ CORNERS

.. - ``mode``  Constant: either CENTER, RADIUS, CORNER, or CORNERS

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	ellipseMode(RADIUS);  // Set ellipseMode to RADIUS
    fill(255);  // Set fill to white
    ellipse(50, 50, 30, 30);  // Draw white ellipse using RADIUS mode

    ellipseMode(CENTER);  // Set ellipseMode to CENTER
    fill(100);  // Set fill to gray
    ellipse(50, 50, 30, 30);  // Draw gray ellipse using CENTER mode
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	ellipseMode(CORNER);  // Set ellipseMode is CORNER
    fill(255);  // Set fill to white
    ellipse(25, 25, 50, 50);  // Draw white ellipse using CORNER mode

    ellipseMode(CORNERS);  // Set ellipseMode to CORNERS
    fill(100);  // Set fill to gray
    ellipse(25, 25, 50, 50);  // Draw gray ellipse using CORNERS mode
	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
