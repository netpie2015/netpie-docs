.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

setMag()
========

Set the magnitude of this vector to the value used for the <b>len</b>
parameter.

**รูปแบบการใช้งาน**

setMag ( len )

**พารามิเตอร์**

- ``len``  : the new length for this vector


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(10, 20, 2);
	// v has components [10.0, 20.0, 2.0]
	v.setMag(10);
	// v's components are set to [6.0, 8.0, 0.0]
	</script>

	<br><br>

.. toctree::

