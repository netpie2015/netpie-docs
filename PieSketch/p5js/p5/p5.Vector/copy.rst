.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

copy()
======

Gets a copy of the vector, returns a p5.Vector object.

**รูปแบบการใช้งาน**

copy ( )

**ค่าที่ส่งออกมา**

- p5.Vector: the copy of the p5.Vector object


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v1 = createVector(1, 2, 3);
	var v2 = v1.copy();
	print(v1.x == v2.x && v1.y == v2.y && v1.z == v2.z);
	// Prints "true"

	</script>

	<br><br>

.. toctree::

