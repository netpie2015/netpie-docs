.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

angleBetween()
==============

คำนวณและส่งกลับค่ามุม (เป็นเรเดียน) ระหว่างสองพาหะ

.. Calculates and returns the angle (in radians) between two vectors.
**รูปแบบการใช้งาน**

angleBetween ( the )

**พารามิเตอร์**

- ``the``  p5.Vector: x, y, และ z ส่วนประกอบของ p5.Vector

.. ``the``  p5.Vector: x, y, and z components of a p5.Vector

**ค่าที่ส่งออกมา**

- Number: มุมระหว่าง (เป็นเรเดียน)

.. Number: the angle between (in radians)

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v1 = createVector(1, 0, 0);
	var v2 = createVector(0, 1, 0);
	
	var angle = v1.angleBetween(v2);
	// angle is PI/2

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
