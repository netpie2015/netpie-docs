.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pmouseY
=========

ตัวแปรระบบ pmouseY จะมีตำแหน่งในแนวตั้งของเมาส์หรือนิ้วในกรอบก่อนเฟรมปัจจุบันเทียบกับ (0, 0) ของผืนผ้าใบ

.. The system variable pmouseY always contains the vertical position of the
.. mouse or finger in the frame previous to the current frame, relative to
.. (0, 0) of the canvas.

**รูปแบบการใช้งาน**

pmouseY

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function draw() {
	  background(237, 34, 93);
	  fill(0);
	  //draw a square only if the mouse is not moving
	  if(mouseY == pmouseY && mouseX == pmouseX)
	    rect(20,20,60,60);
	
	  print(pmouseY + " -> " + mouseY);
	}
	

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
