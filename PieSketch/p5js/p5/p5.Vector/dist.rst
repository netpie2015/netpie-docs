.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

dist()
======

คำนวณระยะทางยุคลิดระหว่างสองจุด (พิจารณาจุดเป็นวัตถุเวกเตอร์)

.. Calculates the Euclidean distance between two points (considering a
.. point as a vector object).
**รูปแบบการใช้งาน**

dist ( v )

**พารามิเตอร์**

- ``v``  p5.Vector: พิกัด x, y และ z ของ p5.Vector

.. ``v``  p5.Vector: the x, y, and z coordinates of a p5.Vector

**ค่าที่ส่งออกมา**

- Number: ระยะทาง

.. Number: the distance

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v1 = createVector(1, 0, 0);
	var v2 = createVector(0, 1, 0);
	
	var distance = v1.dist(v2); // distance is 1.4142...

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Static method
	var v1 = createVector(1, 0, 0);
	var v2 = createVector(0, 1, 0);
	
	var distance = p5.Vector.dist(v1,v2);
	// distance is 1.4142...

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
