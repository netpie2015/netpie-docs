.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

shearX()
========

ตัดเส้นรูปร่างรอบแกน x จำนวนที่กำหนดโดยพารามิเตอร์มุม ควรระบุมุมในมุมฉากปัจจุบัน วัตถุจะถูกตัดรอบตำแหน่งสัมพัทธ์ไปยังต้นกำเนิดและตัวเลขบวกจะตัดวัตถุตามทิศทางตามเข็มนาฬิกา 
การแปลงใช้กับทุกสิ่งทุกอย่างที่เกิดขึ้นหลังจากการโทรไปยังฟังก์ชันนั้นสะสมผล ตัวอย่างเช่นการเรียก shearX (PI / 2) แล้ว shearX (PI / 2) จะเหมือนกับ shearX (PI) ถ้า shearX () ถูกเรียกภายใน draw () การแปลงจะถูกรีเซ็ตเมื่อลูปเริ่มใหม่อีกครั้ง 
เทคนิค shearX () คูณเมทริกซ์การเปลี่ยนแปลงปัจจุบันโดยเมทริกซ์การหมุน ฟังก์ชั่นนี้สามารถควบคุมได้โดยใช้ฟังก์ชั่น push () และ pop ()

.. Shears a shape around the x-axis the amount specified by the angle
.. parameter. Angles should be specified in the current angleMode.
.. Objects are always sheared around their relative position to the origin
.. and positive numbers shear objects in a clockwise direction.
.. 
.. Transformations apply to everything that happens after and subsequent
.. calls to the function accumulates the effect. For example, calling
.. shearX(PI/2) and then shearX(PI/2) is the same as shearX(PI).
.. If shearX() is called within the draw(), the transformation is reset when
.. the loop begins again.
.. 
.. Technically, shearX() multiplies the current transformation matrix by a
.. rotation matrix. This function can be further controlled by the
.. push() and pop() functions.

**รูปแบบการใช้งาน**

shearX ( angle )

**พารามิเตอร์**

- ``angle``  Number: มุมของแรงเฉือนที่ระบุไว้ในเรเดียนหรือองศาขึ้นอยู่กับมุมปัจจุบัน

.. ``angle``  Number: angle of shear specified in radians or degrees, depending on current angleMode

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	translate(width/4, height/4);
	shearX(PI/4.0);
	rect(0, 0, 30, 30);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
