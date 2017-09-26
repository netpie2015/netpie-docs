.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mult()
======

คูณเวกเตอร์ด้วยสเกลาร เวอร์ชันคงที่ของวิธีนี้จะสร้าง p5.Vector ใหม่ในขณะที่เวอร์ชันที่ไม่ใช่แบบคงที่จะทำงานบนเวกเตอร์โดยตรง ดูตัวอย่างสำหรับบริบทเพิ่มเติม

.. Multiply the vector by a scalar. The static version of this method
.. creates a new p5.Vector while the non static version acts on the vector
.. directly. See the examples for more context.

**รูปแบบการใช้งาน**

mult ( n )

**พารามิเตอร์**

- ``n``  Number: จำนวนคูณด้วยเวกเตอร์

.. ``n``  Number: the number to multiply with the vector

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(1, 2, 3);
	v.mult(2);
	// v's components are set to [2, 4, 6]

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// Static method
	var v1 = createVector(1, 2, 3);
	var v2 = p5.Vector.mult(v1, 2);
	// v2 has components [2, 4, 6]

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
