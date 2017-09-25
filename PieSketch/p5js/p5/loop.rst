.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loop()
======

By default, p5.js loops through draw() continuously, executing the code
within it. However, the draw() loop may be stopped by calling noLoop().
In that case, the draw() loop can be resumed with loop().

**รูปแบบการใช้งาน**

loop ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var x = 0;
	function setup() {
	  createCanvas(100, 100);
	  noLoop();
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
	  loop();
	}
	
	function mouseReleased() {
	  noLoop();
	}

	</script>

	<br><br>

.. toctree::

