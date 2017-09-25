.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

atan()
======

The inverse of tan(), returns the arc tangent of a value. This function
expects the values in the range of -Infinity to Infinity (exclusive) and
values are returned in the range -PI/2 to PI/2.

**รูปแบบการใช้งาน**

atan ( value )

**พารามิเตอร์**

- ``value``  Number: the value whose arc tangent is to be returned


**ค่าที่ส่งออกมา**

- Number: the arc tangent of the given value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var a = PI + PI/3;
	var t = tan(a);
	var at = atan(t);
	// Prints: "1.0471976 : 1.7320509 : 1.0471976"
	print(a + " : " + t + " : " +  at);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var a = PI + PI/3.0;
	var t = tan(a);
	var at = atan(t);
	// Prints: "4.1887903 : 1.7320513 : 1.0471977"
	print(a + " : " + t + " : " +  at);

	</script>

	<br><br>

.. toctree::

