.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

degrees()
=========

Converts a radian measurement to its corresponding value in degrees.
Radians and degrees are two ways of measuring the same thing. There are
360 degrees in a circle and 2*PI radians in a circle. For example,
90° = PI/2 = 1.5707964.

**รูปแบบการใช้งาน**

degrees ( radians )

**พารามิเตอร์**

- ``radians``  Number: the radians value to convert to degrees


**ค่าที่ส่งออกมา**

- Number: the converted angle


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var rad = PI/4;
	var deg = degrees(rad);
	print(rad + " radians is " + deg + " degrees");
	// Prints: 0.7853981633974483 radians is 45 degrees


	</script>

	<br><br>

.. toctree::

