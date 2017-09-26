.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

abs()
=====

คำนวณค่าสัมบูรณ์ (ขนาด) ของตัวเลข Maps ไปยัง Math.abs () ค่าสัมบูรณ์ของจำนวนเป็นบวกเสมอ

.. Calculates the absolute value (magnitude) of a number. Maps to Math.abs().
.. The absolute value of a number is always positive.

**รูปแบบการใช้งาน**

abs ( n )

**พารามิเตอร์**

- ``n``  Number: จำนวนที่จะคำนวณ

.. ``n``  Number: number to compute

**ค่าที่ส่งออกมา**

- Number: ค่าสัมบูรณ์ของจำนวนที่ระบุ

.. Number: absolute value of given number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var x = -3;
	  var y = abs(x);
	
	  print(x); // -3
	  print(y); // 3
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
