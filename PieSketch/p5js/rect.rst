.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

rect()
======

วาดรูปสี่เหลี่ยมผืนผ้าไปที่หน้าจอ สี่เหลี่ยมผืนผ้าเป็นรูปสี่เหลี่ยมผืนผ้ามีทุกมุมที่ 90 องศา พารามิเตอร์สองตัวแรกกำหนดตำแหน่งของมุมซ้ายบนส่วนที่สามกำหนดความกว้างและที่สี่กำหนดความสูง วิธีการตีความพารามิเตอร์เหล่านี้อาจเปลี่ยนแปลงได้โดยใช้ฟังก์ชัน rectMode () 
พารามิเตอร์ที่ห้า, หก, เจ็ดและแปดถ้าระบุให้กำหนดรัศมีมุมสำหรับมุมบนขวาล่างซ้ายล่างมุมขวาล่างและมุมล่างซ้ายตามลำดับ พารามิเตอร์รัศมีมุมละเว้นถูกตั้งค่าเป็นค่ารัศมีที่ระบุไว้ก่อนหน้านี้ในรายการพารามิเตอร์

.. Draws a rectangle to the screen. A rectangle is a four-sided shape with
.. every angle at ninety degrees. By default, the first two parameters set
.. the location of the upper-left corner, the third sets the width, and the
.. fourth sets the height. The way these parameters are interpreted, however,
.. may be changed with the rectMode() function.
.. 
.. The fifth, sixth, seventh and eighth parameters, if specified,
.. determine corner radius for the top-right, top-left, lower-right and
.. lower-left corners, respectively. An omitted corner radius parameter is set
.. to the value of the previously specified radius value in the parameter list.

**รูปแบบการใช้งาน**

rect ( x, y, w, h, [tl], [tr], [br], [bl] )

**พารามิเตอร์**

- ``x``  Number: พิกัด x ของสี่เหลี่ยมผืนผ้า

- ``y``  Number: y พิกัดของรูปสี่เหลี่ยมผืนผ้า

- ``w``  Number: ความกว้างของรูปสี่เหลี่ยมผืนผ้า

- ``h``  Number: ความสูงของสี่เหลี่ยมผืนผ้า

- ``tl``  Number: รัศมีทางเลือกของมุมบนซ้าย

- ``tr``  Number: รัศมีเลือกที่มุมบนขวา

- ``br``  Number: รัศมีเลือกที่มุมล่างขวา

- ``bl``  Number: รัศมีเลือกที่มุมล่างซ้าย

.. ``x``  Number: x-coordinate of the rectangle.
.. ``y``  Number: y-coordinate of the rectangle.
.. ``w``  Number: width of the rectangle.
.. ``h``  Number: height of the rectangle.
.. ``tl``  Number: optional radius of top-left corner.
.. ``tr``  Number: optional radius of top-right corner.
.. ``br``  Number: optional radius of bottom-right corner.
.. ``bl``  Number: optional radius of bottom-left corner.

**ค่าที่ส่งออกมา**

- p5: วัตถุ p5

.. p5: the p5 object.

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Draw a rectangle at location (30, 20) with a width and height of 55.
	rect(30, 20, 55, 55);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// Draw a rectangle with rounded corners, each having a radius of 20.
	rect(30, 20, 55, 55, 20);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	// Draw a rectangle with rounded corners having the following radii:
	// top-left = 20, top-right = 15, bottom-right = 10, bottom-left = 5.
	rect(30, 20, 55, 55, 20, 15, 10, 5);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
