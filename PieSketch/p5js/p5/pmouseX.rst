.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pmouseX
=========

ตัวแปรระบบ pmouseX ประกอบด้วยตำแหน่งในแนวนอนของเมาส์หรือนิ้วในเฟรมก่อนเฟรมปัจจุบันเทียบกับ (0, 0) ของผืนผ้าใบ

.. The system variable pmouseX always contains the horizontal position of
.. the mouse or finger in the frame previous to the current frame, relative to
.. (0, 0) of the canvas.

**รูปแบบการใช้งาน**

pmouseX

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Move the mouse across the canvas to leave a trail
	function setup() {
	  //slow down the frameRate to make it more visible
	  frameRate(10);
	}
	
	function draw() {
	  background(244, 248, 252);
	  line(mouseX, mouseY, pmouseX, pmouseY);
	  print(pmouseX + " -> " + mouseX);
	}
	

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
