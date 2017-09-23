.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

keyReleased()
=============

The keyReleased() function is called once every time a key is released.
See key and keyCode for more information.

Browsers may have different default
behaviors attached to various key events. To prevent any default
behavior for this event, add "return false" to the end of the method.

**รูปแบบการใช้งาน**

keyReleased ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function keyReleased() {
	  if (value === 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	  return false; // prevent any default behavior
	}
	</script>

	<br><br>

.. toctree::

