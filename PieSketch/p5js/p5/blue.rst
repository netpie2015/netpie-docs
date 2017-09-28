.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

blue()
======

แยกค่าสีน้ำเงินจากอาร์เรย์สีหรือพิกเซล

.. Extracts the blue value from a color or pixel array.

**รูปแบบการใช้งาน**

blue ( color )

**พารามิเตอร์**

- ``color``  p5.Color,Array: p5.Color object หรือ pixel array

.. ``color``  p5.Color,Array: p5.Color object or pixel array

**ค่าที่ส่งออกมา**

- Number: ค่าสีน้ำเงิน

.. Number: the blue value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	c = color(175, 100, 220);  // Define color 'c'
	fill(c);  // Use color variable 'c' as fill color
	rect(15, 20, 35, 60);  // Draw left rectangle
	
	blueValue = blue(c);  // Get blue in 'c'
	print(blueValue);  // Prints "220.0"
	fill(0, 0, blueValue);  // Use 'blueValue' in new fill
	rect(50, 20, 35, 60);  // Draw right rectangle

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
