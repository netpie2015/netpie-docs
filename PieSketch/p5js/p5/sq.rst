.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

sq()
====

สี่เหลี่ยมจัตุรัสตัวเลข (คูณตัวเลขด้วยตัวเอง) ผลลัพธ์เป็นจำนวนบวกเสมอเนื่องจากการคูณสองจำนวนลบจะให้ผลบวกเสมอ ตัวอย่างเช่น -1 * -1 = 1

.. Squares a number (multiplies a number by itself). The result is always a
.. positive number, as multiplying two negative numbers always yields a
.. positive result. For example, -1 * -1 = 1.

**รูปแบบการใช้งาน**

sq ( n )

**พารามิเตอร์**

- ``n``  Number: จำนวนถึงสี่เหลี่ยมจัตุรัส

.. ``n``  Number: number to square

**ค่าที่ส่งออกมา**

- Number: จำนวนเต็ม

.. Number: squared number

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(200);
	  eSize = 7;
	  x1 = map(mouseX, 0, width, 0, 10);
	  y1 = 80;
	  x2 = sq(x1);
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
	  var spacing = 15;
	  noStroke();
	  fill(0);
	  text("x = " + x1, 0, y1 + spacing);
	  text("sq(x) = " + x2, 0, y2 + spacing);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
