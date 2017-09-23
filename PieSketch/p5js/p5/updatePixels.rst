.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

updatePixels()
==============

Updates the display window with the data in the pixels[] array.
Use in conjunction with loadPixels(). If you're only reading pixels from
the array, there's no need to call updatePixels() — updating is only
necessary to apply changes. updatePixels() should be called anytime the
pixels array is manipulated or set() is called, and only changes made with
set() or direct changes to pixels[] will occur.

**รูปแบบการใช้งาน**

updatePixels ( [x], [y], [w], [h] )

**พารามิเตอร์**

- ``x``  : x-coordinate of the upper-left corner of region to update

- ``y``  : y-coordinate of the upper-left corner of region to update

- ``w``  : width of region to update

- ``h``  : height of region to update


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function preload() {
	  img = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  image(img, 0, 0);
	  var halfImage = 4 * (img.width * pixelDensity()) *
	    (img.height * pixelDensity()/2);
	  loadPixels();
	  for (var i = 0; i < halfImage; i++) {
	    pixels[i+halfImage] = pixels[i];
	  }
	  updatePixels();
	}
	</script>

	<br><br>

.. toctree::

