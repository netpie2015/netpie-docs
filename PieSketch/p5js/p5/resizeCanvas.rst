.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

resizeCanvas()
==============

Resizes the canvas to given width and height. The canvas will be cleared
and draw will be called immediately, allowing the sketch to re-render itself
in the resized canvas.

**รูปแบบการใช้งาน**

resizeCanvas ( w, h, noRedraw )

**พารามิเตอร์**

- ``w``  Number: width of the canvas

- ``h``  Number: height of the canvas

- ``noRedraw``  Boolean: don't redraw the canvas immediately


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

