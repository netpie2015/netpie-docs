.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

width
=======

ความกว้างของภาพ

.. Image width.
**รูปแบบการใช้งาน**

width

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function preload() {
	  img = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  createCanvas(100, 100);
	  image(img, 0, 0);
	  for (var i=0; i < img.width; i++) {
	    var c = img.get(i, img.height/2);
	    stroke(c);
	    line(i, height/2, i, height);
	  }
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
