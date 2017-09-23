.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

textAscent()
============

Returns the ascent of the current font at its current size. The ascent
represents the distance, in pixels, of the tallest character above
the baseline.

**รูปแบบการใช้งาน**

textAscent ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var base = height * 0.75;
	var scalar = 0.8; // Different for each font
	
	textSize(32);  // Set initial text size
	var asc = textAscent() * scalar;  // Calc ascent
	line(0, base - asc, width, base - asc);
	text("dp", 0, base);  // Draw text on baseline
	
	textSize(64);  // Increase text size
	asc = textAscent() * scalar;  // Recalc ascent
	line(40, base - asc, width, base - asc);
	text("dp", 40, base);  // Draw text on baseline
	</script>

	<br><br>

.. toctree::

