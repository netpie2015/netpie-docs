.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

displayDensity()
================

แสดงความหนาแน่นของพิกเซลของการแสดงผลปัจจุบันที่ร่างกำลังทำงานอยู่

.. Returns the pixel density of the current display the sketch is running on.

**รูปแบบการใช้งาน**

displayDensity ( )

**ค่าที่ส่งออกมา**

- Number: ความหนาแน่นของพิกเซลปัจจุบันของจอแสดงผล

.. Number: current pixel density of the display

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

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
