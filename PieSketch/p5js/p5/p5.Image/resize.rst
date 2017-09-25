.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

resize()
========

Resize the image to a new width and height. To make the image scale
proportionally, use 0 as the value for the wide or high parameter.
For instance, to make the width of an image 150 pixels, and change
the height using the same proportion, use resize(150, 0).

**รูปแบบการใช้งาน**

resize ( width, height )

**พารามิเตอร์**

- ``width``  Number: the resized image width

- ``height``  Number: the resized image height


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	
	function setup() {
	  img = loadImage("assets/rockies.jpg");
	}
	function draw() {
	  image(img, 0, 0);
	}
	
	function mousePressed() {
	  img.resize(50, 100);
	}

	</script>

	<br><br>

.. toctree::

