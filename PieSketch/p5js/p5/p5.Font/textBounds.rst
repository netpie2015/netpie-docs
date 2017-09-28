.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

textBounds()
============

ส่งกลับกล่อง bounding แน่นสำหรับสตริงข้อความที่กำหนดโดยใช้แบบอักษรนี้ (ปัจจุบันรองรับเฉพาะบรรทัดเดียวเท่านั้น)

.. Returns a tight bounding box for the given text string using this
.. font (currently only supports single lines)

**รูปแบบการใช้งาน**

textBounds ( line, x, y, fontSize, options )

**พารามิเตอร์**

- ``line``  String: บรรทัดข้อความ

- ``x``  Number: X-ตำแหน่ง

- ``y``  Number: Y-ตำแหน่ง

- ``fontSize``  Number: ขนาดตัวอักษรที่จะใช้ (ตัวเลือก)

- ``options``  Object: ตัวเลือก opiantpe (ตัวเลือก)

.. ``line``  String: a line of text
.. ``x``  Number: x-position
.. ``y``  Number: y-position
.. ``fontSize``  Number: font size to use (optional)
.. ``options``  Object: opentype options (optional)

**ค่าที่ส่งออกมา**

- Object: วัตถุรูปสี่เหลี่ยมผืนผ้าที่มีคุณสมบัติ: x, y, w, h

.. Object: a rectangle object with properties: x, y, w, h

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

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
