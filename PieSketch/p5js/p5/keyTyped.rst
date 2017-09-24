.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

keyTyped()
==========

The keyTyped() function is called once every time a key is pressed, but
action keys such as Ctrl, Shift, and Alt are ignored. The most recent
key pressed will be stored in the key variable.

Because of how operating systems handle key repeats, holding down a key
will cause multiple calls to keyTyped() (and keyReleased() as well). The
rate of repeat is set by the operating system and how each computer is
configured.

Browsers may have different default behaviors attached to various key
events. To prevent any default behavior for this event, add "return false"
to the end of the method.

**รูปแบบการใช้งาน**

keyTyped ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function keyTyped() {
	  if (key === 'a') {
	    value = 255;
	  } else if (key === 'b') {
	    value = 0;
	  }
	  // uncomment to prevent any default behavior
	  // return false;
	}


	</script>

	<br><br>

.. toctree::

