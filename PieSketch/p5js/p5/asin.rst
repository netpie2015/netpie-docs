.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

asin()
======

The inverse of sin(), returns the arc sine of a value. This function
expects the values in the range of -1 to 1 and values are returned
in the range -PI/2 to PI/2.

**รูปแบบการใช้งาน**

asin ( value )

**พารามิเตอร์**

- ``value``  Number: the value whose arc sine is to be returned


**ค่าที่ส่งออกมา**

- Number: the arc sine of the given value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var a = PI + PI/3;
	var s = sin(a);
	var as = asin(s);
	// Prints: "1.0471976 : 0.86602545 : 1.0471976"
	print(a + " : " + s + " : " +  as);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var a = PI + PI/3.0;
	var s = sin(a);
	var as = asin(s);
	// Prints: "4.1887903 : -0.86602545 : -1.0471976"
	print(a + " : " + s + " : " +  as);

	</script>

	<br><br>

.. toctree::

