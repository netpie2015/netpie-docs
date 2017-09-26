.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

winMouseY
===========

ตัวแปรระบบ winMouseY จะมีตำแหน่งแนวตั้งในแนวตั้งของเมาส์โดยสัมพันธ์กับ (0, 0) ของหน้าต่าง

.. The system variable winMouseY always contains the current vertical
.. position of the mouse, relative to (0, 0) of the window.

**รูปแบบการใช้งาน**

winMouseY

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var myCanvas;
	
	function setup() {
	  //use a variable to store a pointer to the canvas
	  myCanvas = createCanvas(100, 100);
	}
	
	function draw() {
	  background(237, 34, 93);
	  fill(0);
	
	  //move the canvas to the vertical mouse position
	  //relative to the window
	  myCanvas.position(windowWidth/2, winMouseY+1);
	
	 //the x of the square is relative to the canvas
	 rect(mouseX,20,60,60);
	}
	

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
