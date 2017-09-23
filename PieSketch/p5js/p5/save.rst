.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

save()
======

Saves the image to a file and force the browser to download it.
Accepts two strings for filename and file extension
Supports png (default) and jpg.

**รูปแบบการใช้งาน**

save ( filename, extension )

**พารามิเตอร์**

- ``filename``  : give your file a name

- ``extension``  : 'png' or 'jpg'


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var photo;
	
	function preload() {
	  photo = loadImage("assets/rockies.jpg");
	}
	
	function draw() {
	  image(photo, 0, 0);
	}
	
	function keyTyped() {
	  if (key == 's') {
	    photo.save("photo", "png");
	  }
	}
	</script>

	<br><br>

.. toctree::

