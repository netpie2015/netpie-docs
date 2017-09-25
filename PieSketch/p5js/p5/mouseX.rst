.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseX
========

The system variable mouseX always contains the current horizontal
position of the mouse, relative to (0, 0) of the canvas. If touch is
used instead of mouse input, mouseX will hold the x value of the most
recent touch point.

**รูปแบบการใช้งาน**

mouseX

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Move the mouse across the canvas
	function draw() {
	  background(244, 248, 252);
	  line(mouseX, 0, mouseX, 100);
	}

	</script>

	<br><br>

.. toctree::

