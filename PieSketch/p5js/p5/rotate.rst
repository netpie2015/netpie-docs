.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

rotate()
========

หมุนรูปร่างจำนวนที่กำหนดโดยพารามิเตอร์มุม ฟังก์ชันนี้ใช้สำหรับมุมองศาเพื่อให้มุมสามารถป้อนได้ทั้งใน RADIANS หรือ DEGREES 
วัตถุหมุนไปรอบ ๆ ตำแหน่งสัมพัทธ์ไปยังต้นทางและจำนวนที่เป็นบวกจะหมุนวัตถุตามเข็มนาฬิกา การแปลงใช้กับทุกสิ่งทุกอย่างที่เกิดขึ้นหลังจากการโทรไปยังฟังก์ชันนั้นสะสมผล ตัวอย่างเช่นการหมุนหมายเลข (HALF_PI) แล้วหมุน (HALF_PI) จะเหมือนกับการหมุน (PI) การปรับเปลี่ยนทั้งหมดจะถูกรีเซ็ตเมื่อวาด () เริ่มต้นอีกครั้ง 
เทคนิคหมุน () คูณเมทริกซ์การเปลี่ยนแปลงปัจจุบันโดยเมทริกซ์การหมุน ฟังก์ชั่นนี้สามารถควบคุมได้โดยกด () และ pop ()

.. Rotates a shape the amount specified by the angle parameter. This
.. function accounts for angleMode, so angles can be entered in either
.. RADIANS or DEGREES.
.. 
.. Objects are always rotated around their relative position to the
.. origin and positive numbers rotate objects in a clockwise direction.
.. Transformations apply to everything that happens after and subsequent
.. calls to the function accumulates the effect. For example, calling
.. rotate(HALF_PI) and then rotate(HALF_PI) is the same as rotate(PI).
.. All tranformations are reset when draw() begins again.
.. 
.. Technically, rotate() multiplies the current transformation matrix
.. by a rotation matrix. This function can be further controlled by
.. the push() and pop().
**รูปแบบการใช้งาน**

rotate ( angle, [axis] )

**พารามิเตอร์**

- ``angle``  Number: มุมของการหมุนที่ระบุไว้ในเรเดียนหรือองศาขึ้นอยู่กับมุมปัจจุบัน

- ``axis``  p5.Vector,Array: (ใน 3d) แกนเพื่อหมุนรอบ

.. ``angle``  Number: the angle of rotation, specified in radians
                       or degrees, depending on current angleMode
.. ``axis``  p5.Vector,Array: (in 3d) the axis to rotate around

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	translate(width/2, height/2);
	rotate(PI/3.0);
	rect(-26, -26, 52, 52);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
