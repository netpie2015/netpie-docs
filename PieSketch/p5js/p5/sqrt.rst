.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

sqrt()
======

คำนวณรากที่สองของจำนวน รากที่สองของจำนวนเป็นบวกแม้ว่าจะมีรากลบที่ถูกต้องก็ตาม รากที่สองของจำนวน a เป็นเช่น s * s = a มันเป็นสิ่งที่ตรงกันข้ามกับการเหลา Maps to Math.sqrt ()

.. Calculates the square root of a number. The square root of a number is
.. always positive, even though there may be a valid negative root. The
.. square root s of number a is such that s*s = a. It is the opposite of
.. squaring. Maps to Math.sqrt().

**รูปแบบการใช้งาน**

sqrt ( n )

**พารามิเตอร์**

- ``n``  Number: จำนวนที่ไม่ใช่เชิงลบต่อรากที่สอง

.. ``n``  Number: non-negative number to square root

**ค่าที่ส่งออกมา**

- Number: รากที่สองของจำนวน

.. Number: square root of number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(200);
	  eSize = 7;
	  x1 = mouseX;
	  y1 = 80;
	  x2 = sqrt(x1);
	  y2 = 20;
	
	  // Draw the non-squared.
	  line(0, y1, width, y1);
	  ellipse(x1, y1, eSize, eSize);
	
	  // Draw the squared.
	  line(0, y2, width, y2);
	  ellipse(x2, y2, eSize, eSize);
	
	  // Draw dividing line.
	  stroke(100)
	  line(0, height/2, width, height/2);
	
	  // Draw text.
	  noStroke();
	  fill(0);
	  var spacing = 15;
	  text("x = " + x1, 0, y1 + spacing);
	  text("sqrt(x) = " + x2, 0, y2 + spacing);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
