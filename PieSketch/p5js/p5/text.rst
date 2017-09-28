.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

text()
======

วาดข้อความไปที่หน้าจอ แสดงข้อมูลที่ระบุในพารามิเตอร์แรกบนหน้าจอในตำแหน่งที่ระบุโดยพารามิเตอร์เพิ่มเติม แบบอักษรเริ่มต้นจะถูกใช้เว้นแต่ว่าจะมีการตั้งค่าแบบอักษรด้วยฟังก์ชัน textFont () และจะใช้ขนาดเริ่มต้นยกเว้นกรณีที่มีการตั้งค่าแบบอักษรด้วย textSize () เปลี่ยนสีของข้อความด้วยฟังก์ชัน fill () เปลี่ยนเค้าโครงของข้อความด้วยฟังก์ชัน stroke () และ strokeWeight () 
ข้อความจะแสดงขึ้นตามความสัมพันธ์กับฟังก์ชัน textAlign () ซึ่งจะมีตัวเลือกให้วาดไปทางซ้ายขวาและตรงกลางของพิกัด 
พารามิเตอร์ x2 และ y2 กำหนดพื้นที่สี่เหลี่ยมเพื่อแสดงภายในและใช้เฉพาะกับข้อมูลสตริงเท่านั้น เมื่อมีการระบุพารามิเตอร์เหล่านี้จะมีการตีความตามการตั้งค่า rectMode () ในปัจจุบัน ข้อความที่ไม่พอดีกับรูปสี่เหลี่ยมผืนผ้าที่ระบุจะไม่ถูกลากไปที่หน้าจอ

.. Draws text to the screen. Displays the information specified in the first
.. parameter on the screen in the position specified by the additional
.. parameters. A default font will be used unless a font is set with the
.. textFont() function and a default size will be used unless a font is set
.. with textSize(). Change the color of the text with the fill() function.
.. Change the outline of the text with the stroke() and strokeWeight()
.. functions.
.. 
.. The text displays in relation to the textAlign() function, which gives the
.. option to draw to the left, right, and center of the coordinates.
.. 
.. The x2 and y2 parameters define a rectangular area to display within and
.. may only be used with string data. When these parameters are specified,
.. they are interpreted based on the current rectMode() setting. Text that
.. does not fit completely within the rectangle specified will not be drawn
.. to the screen.

**รูปแบบการใช้งาน**

text ( str, x, y, [x2], [y2] )

**พารามิเตอร์**

- ``str``  String: สัญลักษณ์ตัวเลขและตัวอักษรที่จะแสดง

- ``x``  Number: x พิกัดของข้อความ

- ``y``  Number: y- พิกัดของข้อความ

- ``x2``  Number: โดยค่าเริ่มต้นความกว้างของกล่องข้อความดู rectMode () สำหรับข้อมูลเพิ่มเติม

- ``y2``  Number: โดยค่าเริ่มต้นความสูงของกล่องข้อความดู rectMode () สำหรับข้อมูลเพิ่มเติม

.. ``str``  String: the alphanumeric symbols to be displayed
.. ``x``  Number: x-coordinate of text
.. ``y``  Number: y-coordinate of text
.. ``x2``  Number: by default, the width of the text box, see rectMode() for more info
.. ``y2``  Number: by default, the height of the text box, see rectMode() for more info

**ค่าที่ส่งออกมา**

- p5: นี้

.. p5: this

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

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
