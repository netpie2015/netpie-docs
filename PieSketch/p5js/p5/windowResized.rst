.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

windowResized()
===============

The windowResized() function is called once every time the browser window
is resized. This is a good place to resize the canvas or do any other
adjustments to accommodate the new window size.

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

.. toctree::

