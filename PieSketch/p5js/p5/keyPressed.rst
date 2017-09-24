.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

keyPressed()
============

The keyPressed() function is called once every time a key is pressed. The
keyCode for the key that was pressed is stored in the keyCode variable.

For non-ASCII keys, use the keyCode variable. You can check if the keyCode
equals BACKSPACE, DELETE, ENTER, RETURN, TAB, ESCAPE, SHIFT, CONTROL,
OPTION, ALT, UP_ARROW, DOWN_ARROW, LEFT_ARROW, RIGHT_ARROW.

For ASCII keys that was pressed is stored in the key variable. However, it
does not distinguish between uppercase and lowercase. For this reason, it
is recommended to use keyTyped() to read the key variable, in which the
case of the variable will be distinguished.

Because of how operating systems handle key repeats, holding down a key
may cause multiple calls to keyTyped() (and keyReleased() as well). The
rate of repeat is set by the operating system and how each computer is
configured.

Browsers may have different default
behaviors attached to various key events. To prevent any default
behavior for this event, add "return false" to the end of the method.

**รูปแบบการใช้งาน**

keyPressed ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function keyPressed() {
	  if (value === 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function keyPressed() {
	  if (keyCode === LEFT_ARROW) {
	    value = 255;
	  } else if (keyCode === RIGHT_ARROW) {
	    value = 0;
	  }
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function keyPressed(){
	  // Do something
	  return false; // prevent any default behaviour
	}


	</script>

	<br><br>

.. toctree::

