.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

random2D()
==========

สร้างเวกเตอร์แบบ 2D ใหม่จากมุมสุ่ม

.. Make a new 2D unit vector from a random angle
**รูปแบบการใช้งาน**

random2D ( )

**ค่าที่ส่งออกมา**

- p5.Vector: วัตถุ p5.Vector ใหม่

.. p5.Vector: the new p5.Vector object

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = p5.Vector.random2D();
	// May make v's attributes something like:
	// [0.61554617, -0.51195765, 0.0] or
	// [-0.4695841, -0.14366731, 0.0] or
	// [0.6091097, -0.22805278, 0.0]

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
