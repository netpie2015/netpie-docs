.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

acos()
======

The inverse of cos(), returns the arc cosine of a value. This function
expects the values in the range of -1 to 1 and values are returned in
the range 0 to PI (3.1415927).

**รูปแบบการใช้งาน**

acos ( value )

**พารามิเตอร์**

- ``value``  : the value whose arc cosine is to be returned


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var a = PI;
	var c = cos(a);
	var ac = acos(c);
	// Prints: "3.1415927 : -1.0 : 3.1415927"
	print(a + " : " + c + " : " +  ac);
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var a = PI + PI/4.0;
	var c = cos(a);
	var ac = acos(c);
	// Prints: "3.926991 : -0.70710665 : 2.3561943"
	print(a + " : " + c + " : " +  ac);
	</script>

	<br><br>

.. toctree::

