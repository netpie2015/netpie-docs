.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

atan2()
=======

คำนวณมุม (เป็นเรเดียน) จากจุดที่ระบุไปยังจุดกำเนิดพิกัดที่วัดจากแกน x บวก ค่าจะถูกส่งคืนเป็นแบบลอยตัวในช่วงตั้งแต่ PI ถึง -PI ฟังก์ชั่น atan2 () มักใช้สำหรับปรับตำแหน่งเรขาคณิตให้อยู่ในตำแหน่งเคอร์เซอร์ 
หมายเหตุ: พิกัด y ของจุดคือพารามิเตอร์ตัวแรกและพิกัด x เป็นพารามิเตอร์ที่สองเนื่องจากโครงสร้างของการคำนวณสัมผัสกัน

.. Calculates the angle (in radians) from a specified point to the coordinate
.. origin as measured from the positive x-axis. Values are returned as a
.. float in the range from PI to -PI. The atan2() function is most often used
.. for orienting geometry to the position of the cursor.
.. 
.. Note: The y-coordinate of the point is the first parameter, and the
.. x-coordinate is the second parameter, due the the structure of calculating
.. the tangent.

**รูปแบบการใช้งาน**

atan2 ( y, x )

**พารามิเตอร์**

- ``y``  Number: y พิกัดของจุด

- ``x``  Number: พิกัด x ของจุด

.. ``y``  Number: y-coordinate of the point
.. ``x``  Number: x-coordinate of the point

**ค่าที่ส่งออกมา**

- Number: สัมผัสอาร์คของจุดที่กำหนด

.. Number: the arc tangent of the given point

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(204);
	  translate(width/2, height/2);
	  var a = atan2(mouseY-height/2, mouseX-width/2);
	  rotate(a);
	  rect(-30, -5, 60, 10);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
