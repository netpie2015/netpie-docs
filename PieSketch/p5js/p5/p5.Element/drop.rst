.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

drop()
======

The .drop() function is called for each file dropped on the element.
It requires a callback that is passed a p5.File object.  You can
optionally pass two callbacks, the first one (required) is triggered
for each file dropped when the file is loaded.  The second (optional)
is triggered just once when a file (or files) are dropped.

**รูปแบบการใช้งาน**

drop ( callback, fxn )

**พารามิเตอร์**

- ``callback``  function: callback triggered when files are dropped.

- ``fxn``  function: callback to receive loaded file.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup() {
	  var c = createCanvas(100, 100);
	  background(200);
	  textAlign(CENTER);
	  text('drop image', width/2, height/2);
	  c.drop(gotFile);
	}
	
	function gotFile(file) {
	  var img = createImg(file.data).hide();
	  // Draw the image onto the canvas
	  image(img, 0, 0, width, height);
	}

	</script>

	<br><br>

.. toctree::

