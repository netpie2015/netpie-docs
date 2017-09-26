.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseY
========

ตัวแปร mouseY ของระบบจะมีตำแหน่งในแนวตั้งของเมาส์อยู่เสมอเมื่อเทียบกับ (0, 0) ของผืนผ้าใบ หากใช้การแตะแทนการป้อนข้อมูลเมาส์ mouseY จะถือค่า y ของจุดสัมผัสล่าสุด

.. The system variable mouseY always contains the current vertical position
.. of the mouse, relative to (0, 0) of the canvas. If touch is
.. used instead of mouse input, mouseY will hold the y value of the most
.. recent touch point.
**รูปแบบการใช้งาน**

mouseY

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Move the mouse across the canvas
	function draw() {
	  background(244, 248, 252);
	  line(0, mouseY, 100, mouseY);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
