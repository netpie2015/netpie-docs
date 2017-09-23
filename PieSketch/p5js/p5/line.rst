.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

line()
======

Draws a line (a direct path between two points) to the screen. The version
of line() with four parameters draws the line in 2D. To color a line, use
the stroke() function. A line cannot be filled, therefore the fill()
function will not affect the color of a line. 2D lines are drawn with a
width of one pixel by default, but this can be changed with the
strokeWeight() function.

**รูปแบบการใช้งาน**

line ( x1, y1, x2, y2 )

**พารามิเตอร์**

- ``x1``  : the x-coordinate of the first point

- ``y1``  : the y-coordinate of the first point

- ``x2``  : the x-coordinate of the second point

- ``y2``  : the y-coordinate of the second point


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	line(30, 20, 85, 75);
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	line(30, 20, 85, 20);
	stroke(126);
	line(85, 20, 85, 75);
	stroke(255);
	line(85, 75, 30, 75);
	</script>

	<br><br>

.. toctree::

