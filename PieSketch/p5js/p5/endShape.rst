.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

endShape()
==========

ฟังก์ชั่น endShape () เป็นตัวช่วยในการเริ่มต้นรูปร่าง () และสามารถเรียกได้เฉพาะหลังจากที่ beginShape () เมื่อเรียกข้อมูล endshape () ข้อมูลภาพทั้งหมดที่กำหนดตั้งแต่การเรียกใช้ครั้งก่อนเพื่อเริ่มต้นรูปร่าง () จะถูกเขียนลงในบัฟเฟอร์ภาพ CLOSE คงที่เป็นค่าสำหรับพารามิเตอร์ MODE เพื่อปิดรูปร่าง (เพื่อเชื่อมต่อจุดเริ่มต้นและจุดสิ้นสุด)

.. The endShape() function is the companion to beginShape() and may only be
.. called after beginShape(). When endshape() is called, all of image data
.. defined since the previous call to beginShape() is written into the image
.. buffer. The constant CLOSE as the value for the MODE parameter to close
.. the shape (to connect the beginning and the end).
**รูปแบบการใช้งาน**

endShape ( [mode] )

**พารามิเตอร์**

- ``mode``  Constant: ใช้ปิดเพื่อปิดรูปร่าง

.. ``mode``  Constant: use CLOSE to close the shape

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	
	beginShape();
	vertex(20, 20);
	vertex(45, 20);
	vertex(45, 80);
	endShape(CLOSE);
	
	beginShape();
	vertex(50, 20);
	vertex(75, 20);
	vertex(75, 80);
	endShape();

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
