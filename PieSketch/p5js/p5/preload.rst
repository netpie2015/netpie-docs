.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

preload()
=========

Called directly before setup(), the preload() function is used to handle
asynchronous loading of external files. If a preload function is
defined, setup() will wait until any load calls within have finished.
Nothing besides load calls should be inside preload (loadImage,
loadJSON, loadFont, loadStrings, etc).

By default the text "loading..." will be displayed. To make your own
loading page, include an HTML element with id "p5_loading" in your
page. More information <a href="http://bit.ly/2kQ6Nio">here</a>.

**รูปแบบการใช้งาน**

preload ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	var c;
	function preload() {  // preload() runs once
	  img = loadImage('assets/laDefense.jpg');
	}
	
	function setup() {  // setup() waits until preload() is done
	  img.loadPixels();
	  // get color of middle pixel
	  c = img.get(img.width/2, img.height/2);
	}
	
	function draw() {
	  background(c);
	  image(img, 25, 25, 50, 50);
	}
	</script>

	<br><br>

.. toctree::

