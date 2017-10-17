.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

green()
=======

แยกค่าสีเขียวจากอาร์เรย์สีหรือพิกเซล

.. Extracts the green value from a color or pixel array.

**รูปแบบการใช้งาน**

green ( color )

**พารามิเตอร์**

- ``color``  p5.Color,Array: p5.Color object หรือ pixel array

.. ``color``  p5.Color,Array: p5.Color object or pixel array

**ค่าที่ส่งออกมา**

- Number: ค่าสีเขียว

.. Number: the green value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	c = color(20, 75, 200);  // Define color 'c'
	fill(c);  // Use color variable 'c' as fill color
	rect(15, 20, 35, 60);  // Draw left rectangle
	
	greenValue = green(c);  // Get green in 'c'
	print(greenValue);  // Print "75.0"
	fill(0, greenValue, 0);  // Use 'greenValue' in new fill
	rect(50, 20, 35, 60);  // Draw right rectangle

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
