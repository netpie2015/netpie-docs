.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

vertex()
========

All shapes are constructed by connecting a series of vertices. vertex()
is used to specify the vertex coordinates for points, lines, triangles,
quads, and polygons. It is used exclusively within the beginShape() and
endShape() functions.

**รูปแบบการใช้งาน**

vertex ( x, y, [z] )

**พารามิเตอร์**

- ``x``  Number: x-coordinate of the vertex

- ``y``  Number: y-coordinate of the vertex

- ``z``  Number,Boolean: z-coordinate of the vertex


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	beginShape(POINTS);
	vertex(30, 20);
	vertex(85, 20);
	vertex(85, 75);
	vertex(30, 75);
	endShape();

	</script>

	<br><br>

.. toctree::

