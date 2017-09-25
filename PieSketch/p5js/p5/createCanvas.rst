.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createCanvas()
==============

Creates a canvas element in the document, and sets the dimensions of it
in pixels. This method should be called only once at the start of setup.
Calling createCanvas more than once in a sketch will result in very
unpredicable behavior. If you want more than one drawing canvas
you could use createGraphics (hidden by default but it can be shown).

The system variables width and height are set by the parameters passed
to this function. If createCanvas() is not used, the window will be
given a default size of 100x100 pixels.

For more ways to position the canvas, see the

positioning the canvas wiki page.

**รูปแบบการใช้งาน**

createCanvas ( w, h, [renderer] )

**พารามิเตอร์**

- ``w``  Number: width of the canvas

- ``h``  Number: height of the canvas

- ``renderer``  Constant: either P2D or WEBGL


**ค่าที่ส่งออกมา**

- HTMLCanvasElement: canvas generated


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  createCanvas(100, 50);
	  background(153);
	  line(0, 0, width, height);
	}

	</script>

	<br><br>

.. toctree::

