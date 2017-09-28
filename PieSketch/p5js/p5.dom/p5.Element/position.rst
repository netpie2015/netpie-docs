.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

position()
==========

ตั้งค่าตำแหน่งขององค์ประกอบที่สัมพันธ์กับ (0, 0) ของหน้าต่าง กำหนดตำแหน่ง: คุณสมบัติสัมบูรณ์และด้านซ้ายและด้านบนของสไตล์ ถ้าไม่มีอาร์กิวเมนต์ให้ส่งกลับตำแหน่ง x และ y ของอิลิเมนต์ในออบเจ็กต์

.. Sets the position of the element relative to (0, 0) of the
.. window. Essentially, sets position:absolute and left and top
.. properties of style. If no arguments given returns the x and y position
.. of the element in an object.

**รูปแบบการใช้งาน**

position ( [x], [y] )

**พารามิเตอร์**

- ``x``  Number: ตำแหน่ง x เทียบกับด้านบนซ้ายของหน้าต่าง

- ``y``  Number: ตำแหน่ง y เทียบกับด้านบนซ้ายของหน้าต่าง

.. ``x``  Number: x-position relative to upper left of window
.. ``y``  Number: y-position relative to upper left of window

**ค่าที่ส่งออกมา**

- Object,p5.Element: 

.. Object,p5.Element: 

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	<code class='norender'>
	function setup() {
	  var cnv = createCanvas(100, 100);
	  // positions canvas 50px to the right and 100px
	  // below upper left corner of the window
	  cnv.position(50, 100);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
