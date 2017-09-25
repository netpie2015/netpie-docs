.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

normalize()
===========

Normalize the vector to length 1 (make it a unit vector).

**รูปแบบการใช้งาน**

normalize ( )

**ค่าที่ส่งออกมา**

- p5.Vector: normalized p5.Vector


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(10, 20, 2);
	// v has components [10.0, 20.0, 2.0]
	v.normalize();
	// v's components are set to
	// [0.4454354, 0.8908708, 0.089087084]

	</script>

	<br><br>

.. toctree::

