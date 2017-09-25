.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

noLoop()
========

Stops p5.js from continuously executing the code within draw().
If loop() is called, the code in draw() begins to run continuously again.
If using noLoop() in setup(), it should be the last line inside the block.

When noLoop() is used, it's not possible to manipulate or access the
screen inside event handling functions such as mousePressed() or
keyPressed(). Instead, use those functions to call redraw() or loop(),
which will run draw(), which can update the screen properly. This means
that when noLoop() has been called, no drawing can happen, and functions
like saveFrame() or loadPixels() may not be used.

Note that if the sketch is resized, redraw() will be called to update
the sketch, even after noLoop() has been specified. Otherwise, the sketch
would enter an odd state until loop() was called.

**รูปแบบการใช้งาน**

noLoop ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  createCanvas(100, 100);
	  background(200);
	  noLoop();
	}
	function draw() {
	  line(10, 10, 90, 90);
	}
	var x = 0;
	function setup() {
	  createCanvas(100, 100);
	}
	
	function draw() {
	  background(204);
	  x = x + 0.1;
	  if (x > width) {
	    x = 0;
	  }
	  line(x, 0, x, height);
	}
	
	function mousePressed() {
	  noLoop();
	}
	
	function mouseReleased() {
	  loop();
	}

	</script>

	<br><br>

.. toctree::

