.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

ellipse()
=========

วาดวงรี (รูปวงรี) ไปที่หน้าจอ วงรีที่มีความกว้างและความสูงเท่ากันคือวงกลม พารามิเตอร์สองตัวแรกกำหนดตำแหน่งและพารามิเตอร์ที่สามและสี่กำหนดความกว้างและความสูงของรูปร่าง หากไม่มีการระบุความสูงค่าความกว้างจะใช้ทั้งความกว้างและความสูง ถ้ามีการระบุความสูงหรือความกว้างเชิงลบจะใช้ค่าสัมบูรณ์ ต้นกำเนิดอาจเปลี่ยนแปลงได้โดยใช้ฟังก์ชัน ellipseMode ()

.. Draws an ellipse (oval) to the screen. An ellipse with equal width and
.. height is a circle. By default, the first two parameters set the location,
.. and the third and fourth parameters set the shape's width and height. If
.. no height is specified, the value of width is used for both the width and
.. height. If a negative height or width is specified, the absolute value is taken.
.. The origin may be changed with the ellipseMode() function.

**รูปแบบการใช้งาน**

ellipse ( x, y, w, [h] )

**พารามิเตอร์**

- ``x``  Number: พิกัด x ของวงรี

- ``y``  Number: พิกัด y ของวงรี

- ``w``  Number: ความกว้างของวงรี

- ``h``  Number: ความสูงของวงรี

.. ``x``  Number: x-coordinate of the ellipse.
.. ``y``  Number: y-coordinate of the ellipse.
.. ``w``  Number: width of the ellipse.
.. ``h``  Number: height of the ellipse.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	ellipse(56, 46, 55, 55);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
