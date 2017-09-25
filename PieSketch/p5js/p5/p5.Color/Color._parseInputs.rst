.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

Color._parseInputs()
====================

For a number of different inputs, returns a color formatted as [r, g, b, a]
arrays, with each component normalized between 0 and 1.

**รูปแบบการใช้งาน**

Color._parseInputs ( [...args] )

**พารามิเตอร์**

- ``...args``  Array: An 'array-like' object that represents a list of arguments


**ค่าที่ส่งออกมา**

- Array.<Number>: a color formatted as [r, g, b, a] Example: input ==> output g ==> [g, g, g, 255] g,a ==> [g, g, g, a] r, g, b ==> [r, g, b, 255] r, g, b, a ==> [r, g, b, a] [g] ==> [g, g, g, 255] [g, a] ==> [g, g, g, a] [r, g, b] ==> [r, g, b, 255] [r, g, b, a] ==> [r, g, b, a]


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// todo

	</script>

	<br><br>

.. toctree::

