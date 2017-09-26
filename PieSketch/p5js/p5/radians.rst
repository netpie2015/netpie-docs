.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

radians()
=========

แปลงการวัดระดับเป็นค่าเรเดียน เรเดียนและองศาเป็นสองวิธีในการวัดสิ่งเดียวกัน มีวงกลม 360 องศาและ 2 * PI เรเดียนในแวดวง ตัวอย่างเช่น 90 ° = PI / 2 = 1.5707964

.. Converts a degree measurement to its corresponding value in radians.
.. Radians and degrees are two ways of measuring the same thing. There are
.. 360 degrees in a circle and 2*PI radians in a circle. For example,
.. 90° = PI/2 = 1.5707964.

**รูปแบบการใช้งาน**

radians ( degrees )

**พารามิเตอร์**

- ``degrees``  Number: ค่าระดับที่จะแปลงเป็นเรเดียน

.. ``degrees``  Number: the degree value to convert to radians

**ค่าที่ส่งออกมา**

- Number: มุมที่แปลง

.. Number: the converted angle

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var deg = 45.0;
	var rad = radians(deg);
	print(deg + " degrees is " + rad + " radians");
	// Prints: 45 degrees is 0.7853981633974483 radians

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
