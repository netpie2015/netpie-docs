.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

textBounds()
============

Returns a tight bounding box for the given text string using this
font (currently only supports single lines)

**รูปแบบการใช้งาน**

textBounds ( line, x, y, fontSize, options )

**พารามิเตอร์**

- ``line``  : a line of text

- ``x``  : x-position

- ``y``  : y-position

- ``fontSize``  : font size to use (optional)

- ``options``  : opentype options (optional)


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var font;
	var textString = 'Lorem ipsum dolor sit amet.';
	function preload() {
	   font = loadFont('./assets/Regular.otf');
	};
	function setup() {
	   background(210);
	
	   var bbox = font.textBounds(textString, 10, 30, 12);
	   fill(255);
	   stroke(0);
	   rect(bbox.x, bbox.y, bbox.w, bbox.h);
	   fill(0);
	   noStroke();
	
	   textFont(font);
	   textSize(12);
	   text(textString, 10, 30);
	};
	</script>

	<br><br>

.. toctree::

