.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

limit()
=======

Limit the magnitude of this vector to the value used for the <b>max</b>
parameter.

**รูปแบบการใช้งาน**

limit ( max )

**พารามิเตอร์**

- ``max``  : the maximum magnitude for the vector


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var v = createVector(10, 20, 2);
	// v has components [10.0, 20.0, 2.0]
	v.limit(5);
	// v's components are set to
	// [2.2271771, 4.4543543, 0.4454354]
	</script>

	<br><br>

.. toctree::

