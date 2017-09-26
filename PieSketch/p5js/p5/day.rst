.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

day()
=====

p5.js สื่อสารกับนาฬิกาบนคอมพิวเตอร์ของคุณ ฟังก์ชันวัน () จะส่งคืนวันที่ปัจจุบันเป็นค่าตั้งแต่ 1 ถึง 31

.. p5.js communicates with the clock on your computer. The day() function
.. returns the current day as a value from 1 - 31.

**รูปแบบการใช้งาน**

day ( )

**ค่าที่ส่งออกมา**

- Number: วันปัจจุบัน

.. Number: the current day

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var d = day();
	text("Current day: \n" + d, 5, 50);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
