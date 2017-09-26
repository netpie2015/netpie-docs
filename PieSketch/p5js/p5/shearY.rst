.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

shearY()
========

ตัดเส้นรูปร่างรอบแกน y จำนวนที่กำหนดโดยพารามิเตอร์มุม ควรระบุมุมในมุมฉากปัจจุบัน วัตถุจะถูกตัดรอบตำแหน่งสัมพัทธ์ไปยังต้นกำเนิดและตัวเลขบวกจะตัดวัตถุตามทิศทางตามเข็มนาฬิกา 
การแปลงใช้กับทุกสิ่งทุกอย่างที่เกิดขึ้นหลังจากการโทรไปยังฟังก์ชันนั้นสะสมผล ตัวอย่างเช่นการเรียก sheary (PI / 2) และ shearY (PI / 2) เหมือนกับ sheary (PI) ถ้า shearY () ถูกเรียกภายใน draw () การแปลงจะถูกรีเซ็ตเมื่อลูปเริ่มต้นอีกครั้ง 
เทคนิค sheary () คูณเมทริกซ์การเปลี่ยนแปลงปัจจุบันโดยเมทริกซ์การหมุน ฟังก์ชั่นนี้สามารถควบคุมได้โดยใช้ฟังก์ชั่น push () และ pop ()

.. Shears a shape around the y-axis the amount specified by the angle
.. parameter. Angles should be specified in the current angleMode. Objects
.. are always sheared around their relative position to the origin and
.. positive numbers shear objects in a clockwise direction.
.. 
.. Transformations apply to everything that happens after and subsequent
.. calls to the function accumulates the effect. For example, calling
.. shearY(PI/2) and then shearY(PI/2) is the same as shearY(PI). If
.. shearY() is called within the draw(), the transformation is reset when
.. the loop begins again.
.. 
.. Technically, shearY() multiplies the current transformation matrix by a
.. rotation matrix. This function can be further controlled by the
.. push() and pop() functions.
**รูปแบบการใช้งาน**

shearY ( angle )

**พารามิเตอร์**

- ``angle``  Number: มุมของแรงเฉือนที่ระบุไว้ในเรเดียนหรือองศาขึ้นอยู่กับมุมปัจจุบัน

.. ``angle``  Number: angle of shear specified in radians or degrees,
                       depending on current angleMode

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	translate(width/4, height/4);
	shearY(PI/4.0);
	rect(0, 0, 30, 30);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
