.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pwinMouseY
============

ตัวแปรของระบบ pwinMouseY จะประกอบด้วยตำแหน่งในแนวตั้งของเมาส์ในกรอบก่อนหน้ากรอบปัจจุบันเทียบกับ (0, 0) ของหน้าต่าง

.. The system variable pwinMouseY always contains the vertical position of
.. the mouse in the frame previous to the current frame, relative to (0, 0)
.. of the window.

**รูปแบบการใช้งาน**

pwinMouseY

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var myCanvas;
	
	function setup() {
	  //use a variable to store a pointer to the canvas
	  myCanvas = createCanvas(100, 100);
	  noStroke();
	  fill(237, 34, 93);
	  }
	
	function draw() {
	  clear();
	  //the difference between previous and
	  //current y position is the vertical mouse speed
	  var speed = abs(winMouseY-pwinMouseY);
	  //change the size of the circle
	  //according to the vertical speed
	  ellipse(50, 50, 10+speed*5, 10+speed*5);
	  //move the canvas to the mouse position
	  myCanvas.position( winMouseX+1, winMouseY+1);
	}
	

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
