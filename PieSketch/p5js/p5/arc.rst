.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

arc()
=====

Draw an arc to the screen. If called with only a, b, c, d, start, and
stop, the arc will be drawn as an open pie. If mode is provided, the arc
will be drawn either open, as a chord, or as a pie as specified. The
origin may be changed with the ellipseMode() function.

Note that drawing a full circle (ex: 0 to TWO_PI) will appear blank
because 0 and TWO_PI are the same position on the unit circle. The
best way to handle this is by using the ellipse() function instead
to create a closed ellipse, and to use the arc() function
only to draw parts of an ellipse.

**รูปแบบการใช้งาน**

arc ( a, b, c, d, start, stop, [mode] )

**พารามิเตอร์**

- ``a``  Number: x-coordinate of the arc's ellipse

- ``b``  Number: y-coordinate of the arc's ellipse

- ``c``  Number: width of the arc's ellipse by default

- ``d``  Number: height of the arc's ellipse by default

- ``start``  Number: angle to start the arc, specified in radians

- ``stop``  Number: angle to stop the arc, specified in radians

- ``mode``  Constant: optional parameter to determine the way of drawing the arc. either CHORD or PIE


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	arc(50, 55, 50, 50, 0, HALF_PI);
	noFill();
	arc(50, 55, 60, 60, HALF_PI, PI);
	arc(50, 55, 70, 70, PI, PI+QUARTER_PI);
	arc(50, 55, 80, 80, PI+QUARTER_PI, TWO_PI);


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	arc(50, 50, 80, 80, 0, PI+QUARTER_PI, OPEN);


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	arc(50, 50, 80, 80, 0, PI+QUARTER_PI, CHORD);


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	arc(50, 50, 80, 80, 0, PI+QUARTER_PI, PIE);


	</script>

	<br><br>

.. toctree::

