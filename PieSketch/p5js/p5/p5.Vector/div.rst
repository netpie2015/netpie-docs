.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

div()
=====

แบ่งเวคเตอร์ด้วยสเกลาร เวอร์ชันคงที่ของวิธีนี้จะสร้าง p5.Vector ใหม่ในขณะที่เวอร์ชันที่ไม่ใช่แบบคงที่จะทำงานบนเวกเตอร์โดยตรง ดูตัวอย่างสำหรับบริบทเพิ่มเติม

.. Divide the vector by a scalar. The static version of this method creates a
.. new p5.Vector while the non static version acts on the vector directly.
.. See the examples for more context.

**รูปแบบการใช้งาน**

div ( n )

**พารามิเตอร์**

- ``n``  number: จำนวนที่จะแบ่งเวคเตอร์ด้วย

.. ``n``  number: the number to divide the vector by

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(6, 4, 2);
	v.div(2); //v's components are set to [3, 2, 1]

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// Static method
	var v1  = createVector(6, 4, 2);
	var v2 = p5.Vector.div(v, 2);
	// v2 has components [3, 2, 1]

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
