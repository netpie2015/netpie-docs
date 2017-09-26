.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

rotate()
========

หมุนเวกเตอร์ตามมุม (เฉพาะเวกเตอร์ 2 มิติ) ขนาดยังคงเหมือนเดิม

.. Rotate the vector by an angle (only 2D vectors), magnitude remains the
.. same

**รูปแบบการใช้งาน**

rotate ( angle )

**พารามิเตอร์**

- ``angle``  number: มุมของการหมุน

.. ``angle``  number: the angle of rotation

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(10.0, 20.0);
	// v has components [10.0, 20.0, 0.0]
	v.rotate(HALF_PI);
	// v's components are set to [-20.0, 9.999999, 0.0]

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
