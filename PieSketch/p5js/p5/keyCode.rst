.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

keyCode
=========

The variable keyCode is used to detect special keys such as BACKSPACE,
DELETE, ENTER, RETURN, TAB, ESCAPE, SHIFT, CONTROL, OPTION, ALT, UP_ARROW,
DOWN_ARROW, LEFT_ARROW, RIGHT_ARROW.
You can also check for custom keys by looking up the keyCode of any key
on a site like this: keycode.info.

**รูปแบบการใช้งาน**

keyCode

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var fillVal = 126;
	function draw() {
	  fill(fillVal);
	  rect(25, 25, 50, 50);
	}
	
	function keyPressed() {
	  if (keyCode == UP_ARROW) {
	    fillVal = 255;
	  } else if (keyCode == DOWN_ARROW) {
	    fillVal = 0;
	  }
	  return false; // prevent default
	}

	</script>

	<br><br>

.. toctree::

