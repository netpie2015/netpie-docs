.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

angleBetween()
==============

Calculates and returns the angle (in radians) between two vectors.

**รูปแบบการใช้งาน**

angleBetween ( the )

**พารามิเตอร์**

- ``the``  : x, y, and z components of a p5.Vector


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v1 = createVector(1, 0, 0);
	var v2 = createVector(0, 1, 0);
	
	var angle = v1.angleBetween(v2);
	// angle is PI/2
	</script>

	<br><br>

.. toctree::

