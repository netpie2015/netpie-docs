.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

fullscreen()
============

ถ้าได้รับอาร์กิวเมนต์ให้กำหนดสเกลให้เต็มหน้าจอหรือไม่ขึ้นอยู่กับค่าอาร์กิวเมนต์ ถ้าอาร์กิวเมนต์ไม่ได้รับจะส่งกลับสถานะปัจจุบันแบบเต็มหน้าจอ โปรดทราบว่าเนื่องจากข้อ จำกัด ของเบราเซอร์นี้สามารถเรียกได้เฉพาะในการป้อนข้อมูลของผู้ใช้ตัวอย่างเช่นเมื่อกดเมาส์เช่นตัวอย่างด้านล่าง

.. If argument is given, sets the sketch to fullscreen or not based on the
.. value of the argument. If no argument is given, returns the current
.. fullscreen state. Note that due to browser restrictions this can only
.. be called on user input, for example, on mouse press like the example
.. below.
**รูปแบบการใช้งาน**

fullscreen ( [val] )

**พารามิเตอร์**

- ``val``  Boolean: ภาพร่างควรอยู่ในโหมดเต็มหน้าจอหรือไม่

.. ``val``  Boolean: whether the sketch should be in fullscreen mode
or not

**ค่าที่ส่งออกมา**

- Boolean: สถานะเต็มหน้าจอปัจจุบัน

.. Boolean: current fullscreen state

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Clicking in the box toggles fullscreen on and off.
	function setup() {
	  background(200);
	}
	function mousePressed() {
	  if (mouseX > 0 && mouseX < 100 && mouseY > 0 && mouseY < 100) {
	    var fs = fullscreen();
	    fullscreen(!fs);
	  }
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
