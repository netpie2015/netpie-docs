.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

height
========

ความสูงของภาพ

.. Image height.

**รูปแบบการใช้งาน**

height

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function preload() {
	  img = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  createCanvas(100, 100);
	  image(img, 0, 0);
	  for (var i=0; i < img.height; i++) {
	    var c = img.get(img.width/2, i);
	    stroke(c);
	    line(0, i, width/2, i);
	  }
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
