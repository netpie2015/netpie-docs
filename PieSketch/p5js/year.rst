.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

year()
======

p5.js สื่อสารกับนาฬิกาบนคอมพิวเตอร์ของคุณ ฟังก์ชันปี () จะส่งคืนปีปัจจุบันเป็นจำนวนเต็ม (2014, 2015, 2016 ฯลฯ )

.. p5.js communicates with the clock on your computer. The year() function
.. returns the current year as an integer (2014, 2015, 2016, etc).

**รูปแบบการใช้งาน**

year ( )

**ค่าที่ส่งออกมา**

- Number: ปีปัจจุบัน

.. Number: the current year

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var y = year();
	text("Current year: \n" + y, 5, 50);

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
