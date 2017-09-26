.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

loadPixels()
============

Loads the pixel data for the display window into the pixels[] array. This
function must always be called before reading from or writing to pixels[].
Note that only changes made with set() or direct manipulation of pixels[]
will occur.

.. Loads the pixel data for the display window into the pixels[] array. This
.. function must always be called before reading from or writing to pixels[].
.. Note that only changes made with set() or direct manipulation of pixels[]
.. will occur.
**รูปแบบการใช้งาน**

loadPixels ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function preload() {
	  img = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  image(img, 0, 0);
	  var d = pixelDensity();
	  var halfImage = 4 * (img.width * d) *
	       (img.height/2 * d);
	  loadPixels();
	  for (var i = 0; i < halfImage; i++) {
	    pixels[i+halfImage] = pixels[i];
	  }
	  updatePixels();
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
