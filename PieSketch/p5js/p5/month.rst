.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

month()
=======

p5.js สื่อสารกับนาฬิกาบนคอมพิวเตอร์ของคุณ ฟังก์ชัน month () จะส่งคืนเดือนปัจจุบันเป็นค่าตั้งแต่ 1 ถึง 12

.. p5.js communicates with the clock on your computer. The month() function
.. returns the current month as a value from 1 - 12.

**รูปแบบการใช้งาน**

month ( )

**ค่าที่ส่งออกมา**

- Number: เดือนปัจจุบัน

.. Number: the current month

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var m = month();
	text("Current month: \n" + m, 5, 50);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
