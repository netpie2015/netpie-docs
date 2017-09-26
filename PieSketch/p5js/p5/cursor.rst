.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

cursor()
========

ตั้งค่าเคอร์เซอร์ไปที่สัญลักษณ์หรือรูปภาพที่กำหนดไว้ล่วงหน้าหรือทำให้ปรากฏหากซ่อนอยู่แล้ว หากคุณพยายามกำหนดภาพเป็นเคอร์เซอร์ขนาดที่แนะนำคือ 16x16 หรือ 32x32 พิกเซล ไม่สามารถโหลดภาพเป็นเคอร์เซอร์หากคุณกำลังส่งออกโปรแกรมของคุณสำหรับเว็บและโหมดทั้งหมดไม่ทำงานกับเบราว์เซอร์ทั้งหมด ค่าสำหรับพารามิเตอร์ x และ y ต้องน้อยกว่าขนาดของภาพ

.. Sets the cursor to a predefined symbol or an image, or makes it visible
.. if already hidden. If you are trying to set an image as the cursor, the
.. recommended size is 16x16 or 32x32 pixels. It is not possible to load an
.. image as the cursor if you are exporting your program for the Web, and not
.. all MODES work with all browsers. The values for parameters x and y must
.. be less than the dimensions of the image.
**รูปแบบการใช้งาน**

cursor ( type, [x], [y] )

**พารามิเตอร์**

- ``type``  String,Constant: ทั้งลูกศร, ข้าม, มือ, MOVE, TEXT, หรือ WAIT หรือเส้นทางสำหรับภาพ

- ``x``  Number: จุดที่ใช้งานอยู่ในแนวนอนของเคอร์เซอร์

- ``y``  Number: จุดที่ใช้งานอยู่ในแนวตั้งของเคอร์เซอร์

.. ``type``  String,Constant: either ARROW, CROSS, HAND, MOVE, TEXT, or
                              WAIT, or path for image
.. ``x``  Number: the horizontal active spot of the cursor
.. ``y``  Number: the vertical active spot of the cursor

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Move the mouse left and right across the image
	// to see the cursor change from a cross to a hand
	function draw() {
	  line(width/2, 0, width/2, height);
	  if (mouseX < 50) {
	    cursor(CROSS);
	  } else {
	    cursor(HAND);
	  }
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
