.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

dot()
=====

คำนวณจุดผลิตภัณฑ์ของสองเวกเตอร์ รุ่นของวิธีการคำนวณจุดผลิตภัณฑ์ของสองเวกเตอร์อิสระเป็นวิธีแบบคงที่ ดูตัวอย่างสำหรับบริบทเพิ่มเติม

.. Calculates the dot product of two vectors. The version of the method
.. that computes the dot product of two independent vectors is a static
.. method. See the examples for more context.
**รูปแบบการใช้งาน**

dot ( x, [y], [z] )

**พารามิเตอร์**

- ``x``  Number,p5.Vector: x ส่วนประกอบของเวกเตอร์หรือ p5.Vector

- ``y``  Number: y องค์ประกอบของเวกเตอร์

- ``z``  Number: z องค์ประกอบของเวกเตอร์

.. ``x``  Number,p5.Vector: x component of the vector or a p5.Vector
.. ``y``  Number: y component of the vector
.. ``z``  Number: z component of the vector

**ค่าที่ส่งออกมา**

- Number: ผลิตภัณฑ์จุด

.. Number: the dot product

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v1 = createVector(1, 2, 3);
	var v2 = createVector(2, 3, 4);
	
	print(v1.dot(v2)); // Prints "20"

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	//Static method
	var v1 = createVector(1, 2, 3);
	var v2 = createVector(3, 2, 1);
	print (p5.Vector.dot(v1, v2)); // Prints "10"

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
