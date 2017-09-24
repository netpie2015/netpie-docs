.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

text()
======

Draws text to the screen. Displays the information specified in the first
parameter on the screen in the position specified by the additional
parameters. A default font will be used unless a font is set with the
textFont() function and a default size will be used unless a font is set
with textSize(). Change the color of the text with the fill() function.
Change the outline of the text with the stroke() and strokeWeight()
functions.

The text displays in relation to the textAlign() function, which gives the
option to draw to the left, right, and center of the coordinates.

The x2 and y2 parameters define a rectangular area to display within and
may only be used with string data. When these parameters are specified,
they are interpreted based on the current rectMode() setting. Text that
does not fit completely within the rectangle specified will not be drawn
to the screen.

**รูปแบบการใช้งาน**

text ( str, x, y, [x2], [y2] )

**พารามิเตอร์**

- ``str``  String: the alphanumeric symbols to be displayed

- ``x``  Number: x-coordinate of text

- ``y``  Number: y-coordinate of text

- ``x2``  Number: by default, the width of the text box, see rectMode() for more info

- ``y2``  Number: by default, the height of the text box, see rectMode() for more info


**ค่าที่ส่งออกมา**

- p5: this


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	textSize(32);
	text("word", 10, 30);
	fill(0, 102, 153);
	text("word", 10, 60);
	fill(0, 102, 153, 51);
	text("word", 10, 90);


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	s = "The quick brown fox jumped over the lazy dog.";
	fill(50);
	text(s, 10, 10, 70, 80); // Text wraps within text box


	</script>

	<br><br>

.. toctree::

