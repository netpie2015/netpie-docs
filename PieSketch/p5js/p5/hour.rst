.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

hour()
======

p5.js สื่อสารกับนาฬิกาบนคอมพิวเตอร์ของคุณ ฟังก์ชัน hour () จะคืนค่าชั่วโมงปัจจุบันเป็นค่าตั้งแต่ 0 ถึง 23

.. p5.js communicates with the clock on your computer. The hour() function
.. returns the current hour as a value from 0 - 23.

**รูปแบบการใช้งาน**

hour ( )

**ค่าที่ส่งออกมา**

- Number: ชั่วโมงปัจจุบัน

.. Number: the current hour

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var h = hour();
	text("Current hour:\n" + h, 5, 50);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
