.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

focused
=========

Confirms if the window a p5.js program is in is "focused," meaning that
the sketch will accept mouse or keyboard input. This variable is
"true" if the window is focused and "false" if not.

**รูปแบบการใช้งาน**

focused

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// To demonstrate, put two windows side by side.
	// Click on the window that the p5 sketch isn't in!
	function draw() {
	  background(200);
	  noStroke();
	  fill(0, 200, 0);
	  ellipse(25, 25, 50, 50);
	
	  if (!focused) {  // or "if (focused === false)"
	    stroke(200,0,0);
	    line(0, 0, 100, 100);
	    line(100, 0, 0, 100);
	  }
	}

	</script>

	<br><br>

.. toctree::

