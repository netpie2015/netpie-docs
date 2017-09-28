.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

degrees()
=========

แปลงการวัดเรเดียนเป็นค่าที่สัมพันธ์กันเป็นองศา เรเดียนและองศาเป็นสองวิธีในการวัดสิ่งเดียวกัน มีวงกลม 360 องศาและ 2 * PI เรเดียนในแวดวง ตัวอย่างเช่น 90 ° = PI / 2 = 1.5707964

.. Converts a radian measurement to its corresponding value in degrees.
.. Radians and degrees are two ways of measuring the same thing. There are
.. 360 degrees in a circle and 2*PI radians in a circle. For example,
.. 90° = PI/2 = 1.5707964.

**รูปแบบการใช้งาน**

degrees ( radians )

**พารามิเตอร์**

- ``radians``  Number: ค่าเรเดียนจะเปลี่ยนเป็นองศา

.. ``radians``  Number: the radians value to convert to degrees

**ค่าที่ส่งออกมา**

- Number: มุมที่แปลง

.. Number: the converted angle

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var rad = PI/4;
	var deg = degrees(rad);
	print(rad + " radians is " + deg + " degrees");
	// Prints: 0.7853981633974483 radians is 45 degrees

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
