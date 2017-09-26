.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

scale()
=======

เพิ่มหรือลดขนาดของรูปร่างโดยการขยายและหดจุด วัตถุมักมีขนาดจากต้นกำเนิดสัมพัทธ์ไปยังระบบพิกัด ค่าสเกลถูกระบุเป็นเปอร์เซ็นต์ทศนิยม ยกตัวอย่างเช่นระดับการเรียกฟังก์ชัน (2.0) จะเพิ่มมิติของรูปร่างขึ้น 200% 
การแปลงใช้กับทุกสิ่งทุกอย่างที่เกิดขึ้นหลังจากและต่อมาเรียกใช้ฟังก์ชันคูณเอฟเฟ็กต์ ตัวอย่างเช่นระดับการโทร (2.0) และระดับ (1.5) จะเหมือนกับขนาด (3.0) ถ้า scale () ถูกเรียกภายใน draw () การแปลงจะถูกรีเซ็ตเมื่อลูปเริ่มใหม่อีกครั้ง 
การใช้ฟังก์ชันนี้กับพารามิเตอร์ z จะใช้ได้เฉพาะในโหมด WEBGL เท่านั้น ฟังก์ชั่นนี้สามารถควบคุมด้วย push () และ pop ()

.. Increases or decreases the size of a shape by expanding and contracting
.. vertices. Objects always scale from their relative origin to the
.. coordinate system. Scale values are specified as decimal percentages.
.. For example, the function call scale(2.0) increases the dimension of a
.. shape by 200%.
.. 
.. Transformations apply to everything that happens after and subsequent
.. calls to the function multiply the effect. For example, calling scale(2.0)
.. and then scale(1.5) is the same as scale(3.0). If scale() is called
.. within draw(), the transformation is reset when the loop begins again.
.. 
.. Using this function with the z parameter is only available in WEBGL mode.
.. This function can be further controlled with push() and pop().

**รูปแบบการใช้งาน**

scale ( s, [y], [z] )

**พารามิเตอร์**

- ``s``  Number,p5.Vector,Array: เปอร์เซ็นต์เพื่อปรับขนาดวัตถุหรือเปอร์เซ็นต์เพื่อปรับขนาดวัตถุในแกน x หากมีการระบุอาร์กิวเมนต์หลายรายการ

- ``y``  Number: เปอร์เซ็นต์เพื่อปรับขนาดวัตถุในแกน y

- ``z``  Number: เปอร์เซ็นต์เพื่อปรับขนาดวัตถุในแกน z (webgl เท่านั้น)

.. ``s``  Number,p5.Vector,Array: percent to scale the object, or percentage to scale the object in the x-axis if multiple arguments are given
.. ``y``  Number: percent to scale the object in the y-axis
.. ``z``  Number: percent to scale the object in the z-axis (webgl only)

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	translate(width/2, height/2);
	rotate(PI/3.0);
	rect(-26, -26, 52, 52);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	rect(30, 20, 50, 50);
	scale(0.5, 1.3);
	rect(30, 20, 50, 50);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
