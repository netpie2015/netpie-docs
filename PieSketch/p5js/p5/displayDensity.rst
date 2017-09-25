.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

displayDensity()
================

Returns the pixel density of the current display the sketch is running on.

**รูปแบบการใช้งาน**

displayDensity ( )

**ค่าที่ส่งออกมา**

- Number: current pixel density of the display


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var density = displayDensity();
	  pixelDensity(density);
	  createCanvas(100, 100);
	  background(200);
	  ellipse(width/2, height/2, 50, 50);
	}

	</script>

	<br><br>

.. toctree::

