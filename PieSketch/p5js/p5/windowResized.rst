.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

windowResized()
===============

ฟังก์ชัน windowResized () เรียกว่าทุกครั้งที่มีการปรับขนาดหน้าต่างเบราเซอร์ นี่เป็นสถานที่ที่ดีในการปรับขนาดของผืนผ้าใบหรือปรับแต่งอื่น ๆ เพื่อรองรับขนาดหน้าต่างใหม่

.. The windowResized() function is called once every time the browser window
.. is resized. This is a good place to resize the canvas or do any other
.. adjustments to accommodate the new window size.
**รูปแบบการใช้งาน**

windowResized ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  createCanvas(windowWidth, windowHeight);
	}
	
	function draw() {
	 background(0, 100, 200);
	}
	
	function windowResized() {
	  resizeCanvas(windowWidth, windowHeight);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
