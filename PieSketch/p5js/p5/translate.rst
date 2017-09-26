.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

translate()
===========

ระบุจำนวนที่จะแทนที่วัตถุภายในหน้าต่างแสดง พารามิเตอร์ x ระบุการแปลแบบซ้าย / ขวาพารามิเตอร์ y ระบุการแปลขึ้น / ลง 
การแปลงจะสะสมและใช้กับทุกสิ่งทุกอย่างที่เกิดขึ้นหลังจากการโทรไปยังฟังก์ชันนั้นสะสมผลกระทบ ตัวอย่างเช่นโทรแปล (50, 0) แล้วแปล (20, 0) เหมือนกับแปล (70, 0) ถ้าแปล () ถูกเรียกภายใน draw () การแปลงจะถูกรีเซ็ตเมื่อลูปเริ่มใหม่อีกครั้ง ฟังก์ชั่นนี้สามารถควบคุมได้โดยใช้ปุ่ม push () และ pop ()

.. Specifies an amount to displace objects within the display window.
.. The x parameter specifies left/right translation, the y parameter
.. specifies up/down translation.
.. 
.. Transformations are cumulative and apply to everything that happens after
.. and subsequent calls to the function accumulates the effect. For example,
.. calling translate(50, 0) and then translate(20, 0) is the same as
.. translate(70, 0). If translate() is called within draw(), the
.. transformation is reset when the loop begins again. This function can be
.. further controlled by using push() and pop().

**รูปแบบการใช้งาน**

translate ( x, y, [z] )

**พารามิเตอร์**

- ``x``  Number: แปลซ้าย / ขวา

- ``y``  Number: แปลขึ้น / ลง

- ``z``  Number: การแปลย้อนหลัง / ย้อนหลัง (เฉพาะ webgl)

.. ``x``  Number: left/right translation
.. ``y``  Number: up/down translation
.. ``z``  Number: forward/backward translation (webgl only)

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	translate(30, 20);
	rect(0, 0, 55, 55);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	rect(0, 0, 55, 55);  // Draw rect at original 0,0
	translate(30, 20);
	rect(0, 0, 55, 55);  // Draw rect at new 0,0
	translate(14, 14);
	rect(0, 0, 55, 55);  // Draw rect at new 0,0

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
