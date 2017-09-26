.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

point()
=======

วาดจุดพิกัดในพื้นที่ที่ขนาดหนึ่งพิกเซล พารามิเตอร์แรกคือค่าแนวนอนสำหรับจุดค่าที่สองคือค่าแนวตั้งสำหรับจุด สีของจุดจะถูกกำหนดโดยจังหวะปัจจุบัน

.. Draws a point, a coordinate in space at the dimension of one pixel.
.. The first parameter is the horizontal value for the point, the second
.. value is the vertical value for the point. The color of the point is
.. determined by the current stroke.

**รูปแบบการใช้งาน**

point ( x, y )

**พารามิเตอร์**

- ``x``  Number: พิกัด x

- ``y``  Number: พิกัด y

.. ``x``  Number: the x-coordinate
.. ``y``  Number: the y-coordinate

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	point(30, 20);
	point(85, 20);
	point(85, 75);
	point(30, 75);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
