.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

resetMatrix()
=============

Replaces the current matrix with the identity matrix.

**รูปแบบการใช้งาน**

resetMatrix ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	translate(50, 50);
	applyMatrix(0.5, 0.5, -0.5, 0.5, 0, 0);
	rect(0, 0, 20, 20);
	// Note that the translate is also reset.
	resetMatrix();
	rect(0, 0, 20, 20);

	</script>

	<br><br>

.. toctree::

