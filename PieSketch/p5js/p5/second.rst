.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

second()
========

p5.js สื่อสารกับนาฬิกาบนคอมพิวเตอร์ของคุณ ฟังก์ชันที่สอง () จะคืนค่าวินาทีปัจจุบันเป็นค่าตั้งแต่ 0 ถึง 59

.. p5.js communicates with the clock on your computer. The second() function
.. returns the current second as a value from 0 - 59.

**รูปแบบการใช้งาน**

second ( )

**ค่าที่ส่งออกมา**

- Number: วินาทีปัจจุบัน

.. Number: the current second

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var s = second();
	text("Current second: \n" + s, 5, 50);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
