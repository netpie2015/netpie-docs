.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

clear()
=======

ล้างพิกเซลภายในบัฟเฟอร์ ฟังก์ชันนี้ใช้งานได้เฉพาะกับวัตถุ p5.Canvas ที่สร้างขึ้นด้วย createCanvas () function; มันจะไม่ทำงานกับหน้าต่างการแสดงผลหลัก พิกเซลในพื้นที่กราฟิกเพิ่มเติมที่สร้างขึ้นด้วย createGraphics () อาจมีความโปร่งใสทั้งหมดหรือบางส่วน ฟังก์ชั่นนี้จะล้างทุกอย่างเพื่อให้ทุกพิกเซลโปร่งใส 100%

.. Clears the pixels within a buffer. This function only works on p5.Canvas
.. objects created with the createCanvas() function; it won't work with the
.. main display window. Unlike the main graphics context, pixels in
.. additional graphics areas created with createGraphics() can be entirely
.. or partially transparent. This function clears everything to make all of
.. the pixels 100% transparent.

**รูปแบบการใช้งาน**

clear ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Clear the screen on mouse press.
	function setup() {
	  createCanvas(100, 100);
	}
	
	function draw() {
	  ellipse(mouseX, mouseY, 20, 20);
	}
	
	function mousePressed() {
	  clear();
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
